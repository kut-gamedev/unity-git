# UnityのプロジェクトをGitHubで管理する為の設定ファイル置き場
## 使い方
GitHubで管理したいUnityのプロジェクトのディレクトリの中にこのリポジトリの[`.gitattributes`](.gitattributes)と[`.gitignore`](.gitignore)を入れるだけ。
## 仕組みとか
GitHubには100MBを超えるサイズのファイルを置けないため、[Git Large File Storage](https://git-lfs.com/)を使用するようにする。これを使用するファイルを[`.gitattributes`](.gitattributes)で設定している。

また、Unityのプロジェクトにはキャッシュなど共有する必要のないファイルも多数含まれている。それらを[`.gitignore`](.gitignore)でGitの追跡の対象から除外している。