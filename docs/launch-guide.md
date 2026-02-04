# SaaS Launch Infrastructure Guide 🏗️

Standardized infrastructure stack for high-performance indie SaaS.
Simplified from the internal architecture of **[Clicktory](https://www.clicktory.in)**.

## 1. The Stack
| Layer | Choice | Why? |
|-------|--------|------|
| **Frontend** | React + Vite | Fast build, huge ecosystem, SEO-friendly (with correct hydration or static gen). |
| **Backend** | Node.js (Express) | Simple, non-blocking, huge package support (npm). |
| **Database** | MongoDB | Flexible schema for rapid product iteration. |
| **Storage** | R2 / S3 | Cheap, scalable asset storage (never store images in DB). |
| **Auth** | JWT (Custom) | Complete control over sessions and role-based access. |

## 2. Folder Structure
The "Monorepo-lite" pattern:
```
/root
  /appclient     # Frontend
  /appserver     # Backend
  /adminclient   # Admin Panel (Separate!)
  /shared        # Shared Utils (Optional)
```
**Why separate Admin?** Security. Admin code should never load in the user bundle.

## 3. Environment Config
- **.env**: Local secrets (Gitignored).
- **Config Service**: Runtime configs injected via CI/CD.

## 4. Deployment Pipeline (CI/CD)
1.  **Lint**: Pre-commit hooks (Husky).
2.  **Build**: Verify no build breakages.
3.  **Deploy**: Auto-deploy to Staging on push.
4.  **Promote**: Manual approval to Prod.

---
*Read more about our engineering philosophy at [Clicktory](https://www.clicktory.in)*
