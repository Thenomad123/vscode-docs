<p align="center">
  <img alt="vscode logo" src="images/logo-stable.png" width="100px" />
  <h1 align="center">Visual Studio Code Documentation</h1>
</p>

You've found the Visual Studio Code documentation GitHub repository, which contains the content for the [Visual Studio Code documentation](https://code.visualstudio.com/docs).

Topics submitted here will be published to the [Visual Studio Code](https://code.visualstudio.com) portal.

If you are looking for the VS Code product GitHub repository, you can find it [here](https://github.com/microsoft/vscode).

>**Note**: The vscode-docs repository uses [Git LFS](https://git-lfs.github.com/) (Large File Storage) for storing binary files such as images and `.gif`s. If you are contributing or updating images, please enable Git LFS per the instructions in the [Contributing](#cloning) section below.

## Index

- [Index](#index)
- [Visual Studio Code](#visual-studio-code)
- [Feedback](#feedback)
- [Documentation Issues](#documentation-issues)
- [Contributing](#contributing)
  - [Workflow](#workflow)
  - [Cloning](#cloning)
    - [Cloning without binary files](#cloning-without-binary-files)
- [Publishing](#publishing)

## Visual Studio Code

[VS Code](https://code.visualstudio.com/) is a lightweight source code editor and powerful development environment for building and debugging modern web, mobile, and cloud applications. It is free and available on your favorite platform - Linux, macOS, and Windows.

If you landed here looking for other information about VS Code, head over to [our website](https://code.visualstudio.com) for additional information.

## Feedback

If you want to give documentation feedback, please use the feedback control located at the bottom of each documentation page.

## Documentation Issues

To enter documentation bugs, please create a [new GitHub issue](https://github.com/microsoft/vscode-docs/issues). Please check if there is an existing issue first.

If you think the issue is with the VS Code product itself, please enter issues in the VS Code product repo [here](https://github.com/microsoft/vscode/issues).

## Contributing

To contribute new topics/information or make changes to existing documentation, please read the [Contributing Guideline](./CONTRIBUTING.md#contributing).

### Workflow

The two suggested workflows are:

- For small changes, use the "Edit" button on each page to edit the Markdown file directly on GitHub.
- If you plan to make significant changes or preview the Markdown files in VS Code, [clone](#cloning) the repo to [edit and preview](https://code.visualstudio.com/docs/languages/markdown) the files directly in VS Code.

![Markdown Preview Button](images/MDPreviewButton.png)

### Cloning

1. Install [Git LFS](https://git-lfs.github.com/).
2. Run `git lfs install` to setup global git hooks. You only need to run this once per machine.
3. SSH auth: `git clone git@github.com:microsoft/vscode-docs.git`<br>HTTPS auth: `git clone https://github.com/microsoft/vscode-docs.git`
4. Now you can `git add` binary files and commit them. They'll be tracked in LFS.

#### Cloning without binary files

You might want to clone the repo without the 1.6GB images. Here are the steps:

1. Install [Git LFS](https://git-lfs.github.com/).
2. Run `git lfs install` to setup global git hooks. You only need to run this once per machine.
3. Clone the repo without binary files.
    - macOS / Linux:
      - SSH auth: `GIT_LFS_SKIP_SMUDGE=1 git clone git@github.com:microsoft/vscode-docs.git`
      - HTTPS auth: `GIT_LFS_SKIP_SMUDGE=1 git clone https://github.com/microsoft/vscode-docs.git`
    - Windows:
      - SSH auth: `$env:GIT_LFS_SKIP_SMUDGE="1"; git clone git@github.com:microsoft/vscode-docs.git`
      - HTTPS auth: `$env:GIT_LFS_SKIP_SMUDGE="1"; git clone https://github.com/microsoft/vscode-docs.git`
4. Now you can selectively checkout some binary files to work with. For example:
    - `git lfs pull -I "docs/nodejs"` to only download images in `docs/nodejs`
    - `git lfs pull -I "release-notes/images/1_4*/*"` to only download images in `release-notes/images/1_4*`
    - `git lfs pull -I "docs,api"` to download all images in `docs` and in `api`
    - `git lfs pull -I <PATTERN>`, as long as `<PATTERN>` is a valid [Git LFS Include and Exclude pattern](https://github.com/git-lfs/git-lfs/blob/main/docs/man/git-lfs-fetch.adoc#include-and-exclude).

The history of this repo before we adopted LFS can be found at [microsoft/vscode-docs-archive](https://github.com/microsoft/vscode-docs-archive).

## Publishing

Publishing merged pull requests is not automatic and is initiated manually after changes have been reviewed on an internal staging server. There is no specific time guarantee for when PR updates will be available on https://code.visualstudio.com but the intent is that they will usually be live within 24 hours.

3000A32221C10100010F01F60600018000580333320C057D7D0504303C32DD10D2001E020000567F0000A0
300235506BF0F0F0F0212B35578AF0F0141B21304671F0546594281EFFFFFFFFFFFFFFFFFFFFFFFFFFFFAA
30030A14050712320A200305BE7D69646E1E28205D39093FFE3FFE0715010C0C0C0C01050A141E461E01504E1703AA
3500FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
3501FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
3502FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
3503FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
3504FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
3505FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
3506FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
3507FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
3508FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
3509FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
350AFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
350BFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
350CFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
350DFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
350EFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
350FFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF
3510404221008FF7FCFD112A0001FEEEFFF7
35110A400800BBFEF7FF68944010D1FFFFF7
35124B280012FFF7FFFD42150000FDFFF7FF
351340104208BFFEE7FF001300639EFFFFFE
35142C200112B2A37FFF95B27400FDFEDDFF
35152B000000FFFFB9EE0A450000FE7EFDBE
351610C600007FBFFFEF6E004418FFDFEF7F
351725410200F1DFFFFF8DD00018B9FBFDFF
35209A019001500A01143B012501030A280014286400111C3900145064322D28281E1E19140019323C465A78C850504D4946413C32000032003648
3521050A141E28323C50020F2D4C5F5F5F5F5F5F5F5F4F50514F4848494940424343393A3D3C3033363600182627
3522000306112200365AA2000000000028320A003C503200646464006464640A141E3246005AA2646464646464646464646464646464
352300050F1E283241505A646E8296B4C8FAC891877D7A776F6C645C554B351D030000050F1E283241505A646E8296B4C8FAC891877D7A776F6C645C554B351D0300
10111664020B1701C00C085064
10123033303047435357
1014000806FF
3000117C024D381E1E320F0E081E88007F00000000
30016AF9A1060200100218000000000000000000000000000000
30020000F07FBF002323052333190F051E14000A000000
300360051408083C280019020000
3004800505140209AA280E3203012000
3005570A05270000
300600000000
