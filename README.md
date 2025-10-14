# Medical Imaging Symposium webpage

Repo for [medimagesymposium.github.io](https://medimagesymposium.github.io/).

Structure:
```
.
├── assets/
│   ├── css/
│   │   └── style.css
│   ├── images/
│   │   └── 2024/
│   │   └── some_image.png
│   └── booklets/
│       └── previous_edition.pdf
├── _includes/
├── _layouts_/
├── _pages/
│   ├── previous/
│   │   └── 2024.markdown
│   │   └── 2025.markdown
│   └── about.markdown
│   └── index.markdown
```

- `_pages`: contains the contents of the webpage in markdown format
- `_layouts` and `_includes`: define the webpage format
- `assets`: contains images, documents, styles, etc.

## Local development

See [Testing your GitHub Pages site locally with Jekyll](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/testing-your-github-pages-site-locally-with-jekyll).

For Windows specifically (as explained [here](https://jekyllrb.com/docs/installation/windows/)) :
1. Download and install a Ruby+Devkit version from [RubyInstaller Downloads](https://rubyinstaller.org/downloads/). Use default options for installation.
2. Run the `ridk install` step on the last stage of the installation wizard. This is needed for installing gems with native extensions. You can find additional information regarding this in the [RubyInstaller Documentation](https://github.com/oneclick/rubyinstaller2#using-the-installer-on-a-target-system). From the options choose `MSYS2 and MINGW development toolchain`.
3. Open a new command prompt window from the start menu, so that changes to the `PATH` environment variable becomes effective. Install Jekyll and Bundler using `gem install jekyll bundler`.

Then, use [VS Code](https://code.visualstudio.com/) to make use of the `Install bundle` and `Start Jekyll` tasks defined in `.vscode\tasks.json`. Invoke them with `Ctrl+Shift+P` `->` `Run Task`.