# Grid++ Template

Fork 這個 repository，再 clone 自己的 fork。請先依照 [Grid++ 文件](https://gridplusplus.github.io/GridPlusPlus/01-getting-started/01-installation/)安裝 raylib。

## 編譯

Linux／WSL：

```bash
g++ -std=c++17 main.cpp -o game -lraylib -lGL -lm -lpthread -ldl -lrt -lX11
```

macOS：

```bash
g++ -std=c++17 main.cpp -o game $(pkg-config --cflags --libs raylib)
```

Windows／MinGW-w64：

```bash
g++ -std=c++17 main.cpp -o game.exe -Iraylib/include -Lraylib/lib -lraylib -lgdi32 -lwinmm
```

需要新版 Grid++ 時，在 GitHub fork 首頁按 **Sync fork**。推送至課程 Gitea 後，Actions 會自動建立 WASM 網頁。
