# Contributor instructions

- Sign every Git commit with the configured backend and key. If signing fails, preserve the uncommitted files. Verify each new commit and report verifier or trust configuration issues. Use English commit messages.
- Use Allman braces for functions, block-bodied arrows, methods, accessors, constructors, and type and class declarations. Keep existing control-flow style. Preserve language syntax and align any formatter with this convention.
- Keep real vault files, file inventories, and service credentials out of source and test fixtures.
- Keep the initial inventory probe read-only. FolderSync remains active in the test vault and delivers the unpublished build to Android.
- Test kDrive API updates against a dedicated test folder and verify file history in the kDrive web interface.
- Verify both Windows and Android before enabling bidirectional writes in a live vault.
