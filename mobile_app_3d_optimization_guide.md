# B Socio AR Studio: Mobile App & 3D Optimization Settings

## 1. Mobile App Manifest (Android/iOS)
To ensure a native-like experience when packaged via Capacitor or React Native.

### App Identification
- **App Name**: B Socio AR Studio
- **Package ID**: `in.bsocio.arstudio`
- **Primary Icon**: {{DATA:IMAGE:IMAGE_40}} (Hexagonal Monogram)
- **Splash Screen**: #11131c background with centered {{DATA:IMAGE:IMAGE_40}}

### Required Permissions
- `CAMERA`: Required for AR tracking and marker detection.
- `INTERNET`: Required for fetching 3D assets from CDN.
- `WRITE_EXTERNAL_STORAGE`: Optional, for saving AR screenshots/recordings.

---

## 2. 3D Asset Optimization Parameters
Standardized settings for high-performance mobile WebXR rendering.

### Geometry & Meshes
- **Format**: glTF 2.0 (.glb) with Drace compression.
- **Poly Count Limit**: 
  - Standard Mobile: < 100,000 triangles.
  - High-End Mobile: < 250,000 triangles.
- **Draw Calls**: Aim for < 50 per scene to maintain 60 FPS.

### Textures & Materials
- **Resolution**: 1024x1024 (2048x2048 only for hero assets).
- **Format**: Basis Universal (KHK) or WebP for GPU compression.
- **Shaders**: Use PBR (Physically Based Rendering) standard materials.

### Animation
- **Limit**: Max 5 animation clips per model.
- **Bones**: Max 64 bones for rigged characters to ensure compatibility with older mobile GPUs.

---

## 3. Global Edge Configuration
- **CDN**: CloudFront with Origin Shield.
- **Caching**: 1 year (Immutable) for 3D assets via hash-based URLs.
- **Compression**: Brotli encoding enabled for all JSON/HTML/JS payloads.