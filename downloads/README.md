# Downloads Folder

This folder contains smaller files that are part of the website. 

## Large Files Storage

Large files (PDFs, presentations, etc.) have been moved to a separate branch called `downloads-storage` to keep the main website repository lightweight.

### Accessing Large Files

All large files can be accessed via GitHub raw URLs using the format:
```
https://github.com/fewbody/fewbody.github.io/raw/downloads-storage/FILENAME
```

For example:
- `https://github.com/fewbody/fewbody.github.io/raw/downloads-storage/np_bound_numerov.pdf`
- `https://github.com/fewbody/fewbody.github.io/raw/downloads-storage/seminar-tongji-2025-nogga.pdf`

### For Developers

To update or add large files:
1. Switch to the `downloads-storage` branch: `git checkout downloads-storage`
2. Add your files and commit them to that branch
3. Use the GitHub raw URL pattern above to link to files from the website

This approach keeps the main website deployment under GitHub's size limits while preserving access to all files.