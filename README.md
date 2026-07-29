# LA Tennis Court Finder — Build 11 immediate exit

This build removes the launch finalization screen from the execution path.

After the fifth calibration location:

1. Court detection is enabled synchronously.
2. The launch overlay is hidden synchronously.
3. The main map is rendered immediately.
4. Satellite descriptor extraction continues in the background.
5. Calibration-map cleanup happens only after the site is visible.

There is no awaited promise, progress loop, animation, or network request
between the fifth click and opening the main map.

## Confirming the deployed version

The launch screen says:

```text
Detector setup · Build 11
```

An older screen without `Build 11`, or one that says
`Applying your court pins`, is a cached or older deployment.

## Deploy

Delete or overwrite the existing repository files, upload every file from this
folder to the repository root, and commit to `main`.

GitHub Pages should publish from `main` and `/ (root)`.
