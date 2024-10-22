# Fooocus向けプリセットファイル

[Fooocus](https://github.com/lllyasviel/Fooocus/) 向けの追加プリセットファイルです。

モデルをインストールする手間が省けたり、Fooocus起動時のモデルを変更できます。

## プリセット一覧

アニメ・マンガ系モデルがあります。

いずれも初期サイズ 1024 x 1024 、スタイルなしです。

| プリセット | モデル | VAE | CFG Scale |
| ---- | ---- | ---- | ---- |
| aam | AAM(Anime Mix) | - | 6 |
| animagine | Animagine | SDXL-VAE | 6 |
| cheyenne | CHEYENNE | SDXL-VAE | 5 |

## インストール

.json ファイルを <FOOOCUS_HOME>/presets ディレクトリに配置してください。

## Fooocus起動時のプリセット指定

Fooocus起動時にプリセットを指定するには `--preset` オプションの引数にプリセット名を指定してください。

以下はプリセット animagine を使用する例です。

```例：Mac
python entry_with_update.py --preset animagine
```

```例：Google Colab
!python entry_with_update.py --share --always-high-vram --preset animagine
```
Windows 版は `run_animagine.bat` のような.batファイルを作成してください。

```例：Windows（run_animagine.bat）
.\python_embeded\python.exe -s Fooocus\entry_with_update.py --preset animagine
pause
```

