# Continuum Sync

An Obsidian plugin for bidirectional vault sync with cloud storage you control. The plugin ID is `continuum-sync`. The first backend will use the native kDrive API.

## Development

Start with a read-only inventory in Obsidian on Windows and Android. Inventory should account for hidden files, configuration, and attachments. Vault-relative path rules determine which files are excluded from sync.

FolderSync stays active in the test vault and delivers the unpublished plugin build to Android. The inventory probe reports what Obsidian can enumerate and read. The next milestone verifies, in a dedicated kDrive test folder, that updates preserve the version history of the existing file.

Bidirectional sync follows after those checks. Initial reconciliation needs a preview. Interrupted jobs must resume safely, conflicting edits must preserve both versions, and exclusions must never cause a deletion.
