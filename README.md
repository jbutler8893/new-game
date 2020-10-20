# new-game
- name: Cache
  uses: actions/cache@v2.1.2
  with:
    # A list of files, directories, and wildcard patterns to cache and restore
    path: 
    # An explicit key for restoring and saving the cache
    key: 
    # An ordered list of keys to use for restoring the cache if no cache hit occurred for key
    restore-keys: # optional
    # The chunk size used to split up large files during upload, in bytes
    upload-chunk-size: # optional
    - name: Upload a Build Artifact
  uses: actions/upload-artifact@v2.2.0
  with:
    # Artifact name
    name: # optional, default is artifact
    # A file, directory or wildcard pattern that describes what to upload
    path: 
    # The desired behavior if no files are found using the provided path.
Available Options:
  warn: Output a warning but do not fail the action
  error: Fail the action with an error message
  ignore: Do not output any warnings or errors, the action does not fail

    if-no-files-found: # optional, default is warn
    # Duration after which artifact will expire in days. 0 means using default retention.
Minimum 1 day. Maximum 90 days unless changed from the repository settings page.

    retention-days: # optional
