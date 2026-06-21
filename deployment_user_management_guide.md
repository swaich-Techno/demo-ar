# B Socio AR Studio: Deployment & Management Guide

## 1. Deployment Overview
B Socio AR Studio is built on a modern full-stack architecture designed for high-performance 3D rendering and global scalability.

### Web Deployment
- **Frontend**: Deploy the React/Tailwind build to **Vercel** or **Netlify** for edge-node performance.
- **Subdomains**: Map `ar.bsocio.in` as the primary control hub. Experiences are served via `experiences.bsocio.in/project-id`.

### Mobile Application (Android/iOS)
- **Wrapper**: Use **Capacitor** or **React Native WebView** to package the web application.
- **Icon**: Use the hexagonal "AR" monogram ({{DATA:IMAGE:IMAGE_40}}) as the app icon for all platforms.
- **AR Engine**: Ensure the mobile app has permissions for **Camera Access** and **WebGL 2.0**.

---

## 2. Team & Administrative Access

### Super Admin (Full Control)
The Super Admin is the root user responsible for global system health and master approvals.
- **Login URL**: `ar.bsocio.in/admin/login` ({{DATA:SCREEN:SCREEN_107}})
- **Capabilities**: Global user management, system health monitoring, and enterprise seat allocation.
- **Creation**: Initial Super Admin is created via a secure CLI script during database initialization:
  `npm run create:super-admin -- --email="admin@bsocio.in" --pass="secure_password"`

### B Socio Team Logins
Internal team members (Creators, Editors, Viewers) use the specialized team portal.
- **Login URL**: `ar.bsocio.in/team/login` ({{DATA:SCREEN:SCREEN_35}})
- **Onboarding**: Team members are invited via the **Enterprise User Permissions** module ({{DATA:SCREEN:SCREEN_79}}). 
- **Roles**:
  - **Admin**: Manage team members and publish campaigns.
  - **Creator**: Access AR Studio and VFX tools.
  - **Viewer**: Read-only access to analytics and previews.

---

## 3. Production Launch Checklist
1. **SSL Certificates**: Provision Wildcard SSL via Let's Encrypt for all subdomains.
2. **Asset CDN**: Configure an S3 bucket with CloudFront for high-speed 3D model (glTF) delivery.
3. **Database**: Switch from local SQLite to a production-grade PostgreSQL instance.
4. **Environment**: Update all `NEXT_PUBLIC_BASE_URL` variables to point to the live domains.

---

## 4. How to Use the Studio
1. **Login**: Access the dashboard via your designated portal.
2. **Create**: Use the **AR Studio** ({{DATA:SCREEN:SCREEN_52}}) to upload assets or use templates.
3. **Interactivity**: Add logic via the **Scene Interactivity Studio** ({{DATA:SCREEN:SCREEN_85}}).
4. **Deploy**: Generate a QR code in the **Batch QR Generator** ({{DATA:SCREEN:SCREEN_26}}).
5. **Analyze**: Monitor performance in real-time via the **Analytics Portal** ({{DATA:SCREEN:SCREEN_42}}).