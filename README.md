# Today I Learned

Collection of TIL tidbits

## Git

- Use `includeIf` directive to conditionally set git credentials based on project location on disk - [conditional credentials](https://dev.to/tastefulelk/conditional-git-profile-configuration-212b)

## VS Code

- You can configure a set of "Recommended" extensions for a project that will be suggested to other users of the same project - [Recommended Extensions](https://code.visualstudio.com/docs/editor/extension-marketplace#_recommended-extensions)
- Alias `code ,` to `code .` to stop constantly accidentally opening an empty file instead of CWD. Add the following to `.zshrc` or equivalent:

  ```sh
  code() {
    if [[ $@ == "," ]]; then
        command code .
    else
        command code "$@"
    fi
  }
  ```
