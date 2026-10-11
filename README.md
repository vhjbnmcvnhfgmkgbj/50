# SnapRelay fixed project

## GitHub upload
Upload all contents of this folder to your repository root. Create the workflow file at `.github/workflows/Build.yml` using `.github-workflow.yml` from this package. Replace `YOUR-HTTPS-SERVER.example.com` in `android/app/src/main/java/com/snaprelay/app/MainActivity.kt` with your HTTPS server URL.

## Fix included
`MainActivity.kt` now imports OkHttp's `toMediaType()` and `toRequestBody()` extensions, which were missing and caused the Kotlin build to fail.
