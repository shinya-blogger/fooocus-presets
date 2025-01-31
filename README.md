# Fooocus向けプリセットファイル

[Fooocus](https://github.com/lllyasviel/Fooocus/) 向けの追加プリセットファイルです。

モデルをインストールする手間が省けたり、Fooocus起動時のモデルを変更できます。

## プリセット一覧

アニメ・マンガ系モデルがあります。

いずれも初期サイズ 1024 x 1024 、スタイルなしです。

バージョン番号なしのプリセットは最新版を指します。

| プリセット | モデル | VAE | CFG Scale |
| ---- | ---- | ---- | ---- |
| aam | AAM(Anime Mix) v1.0 | - | 6 |
| aam_v1.0 | AAM(Anime Mix) v1.0 | - | 6 |
| animagine | Animagine XL 4.0 | SDXL-VAE | 6 |
| animagine_v4.0 | Animagine XL 4.0 | SDXL-VAE | 6 |
| animagine_v3.1 | Animagine XL 3.1 | SDXL-VAE | 6 |
| cheyenne | CHEYENNE v2.0 | SDXL-VAE | 5 |
| cheyenne_v2.0 | CHEYENNE v2.0 | SDXL-VAE | 5 |
| cheyenne_v1.8 | CHEYENNE v1.8 | SDXL-VAE | 5 |

## インストール

.json ファイルを <FOOOCUS_HOME>/presets ディレクトリに配置してください。

## Fooocus起動時のプリセット指定

Fooocus起動時にプリセットを指定するには `--preset` オプションの引数にプリセット名を指定してください。

以下はプリセット animagine_v4.0 を使うときの起動方法の例です。

### Windows
Windows 版は `run_animagine.bat` のような .bat ファイルを作成してください。

```例：Windows（run_animagine.bat）
.\python_embeded\python.exe -s Fooocus\entry_with_update.py --preset animagine_v4.0
pause
```

### Mac

```
python entry_with_update.py --preset animagine_v4.0
```

### Google Colab
```
!python entry_with_update.py --share --always-high-vram --preset animagine_v4.0
```

