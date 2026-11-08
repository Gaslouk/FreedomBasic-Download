# Freedom Basic

Freedom Basic is a BASIC interpreter and IDE for Windows that aims to be compatible with **Liberty BASIC 4.5.1**. Existing Liberty BASIC programs (windows, graphicboxes, dialogs, files and the usual statements) are meant to run as they are. Compatibility is checked by comparing Freedom Basic's behaviour with the real Liberty BASIC.

**Free to try for one year.** See [Licensing](#licensing) below.

## Download

Get the latest files from the [Releases](../../releases) page:

| File | What it is |
|---|---|
| `FreedomBasic64.exe` | The IDE, 64-bit (recommended) |
| `FreedomBasic32.exe` | The IDE, 32-bit |
| `FreedomBasic_Linux_b638.tar.gz` | Linux (x86-64): runs programs, includes the Designer, no editor window |
| `FreedomDesigner.1.42_LB.zip` | The form designer, with its `icons` folder |
| `freedombasic_help.zip` | Offline help (English and Greek), open `pages/index.html`; also in the `freedombasic_help` folder of this repository |

No installation is needed, and the Microsoft Visual C++ Redistributable is **not** required. Save the exe anywhere and run it.

## Features

- IDE with editor, Run and Debug
- `$INCLUDE` support
- Builds standalone `.exe` files from your programs (licensed versions, and during the free year)
- A form designer written in Freedom Basic itself (see below)

## Linux

```
tar xzf FreedomBasic_Linux_b638.tar.gz
cd FreedomBasic_Linux_b638
./freedom program.bas
```

The package includes the SDL3 libraries, the Designer (`./freedom-designer`) and an example game. It needs a 64-bit Linux desktop. The Linux package runs programs; it has no editor window and no license limits.

## Freedom Designer

The designer lets you place controls on a form with the mouse and generates the Liberty BASIC code for it.

1. Unzip `FreedomDesigner.*_LB.zip`. Keep the `icons` folder **next to** the designer, with its `.bmp` files directly inside it. Without it the palette still works, but without pictures.
2. Run the designer with Freedom Basic. It uses a few Freedom Basic extensions, so it does **not** run on Liberty BASIC.
3. Drag the splitter above the code tabs to resize the code pane.

## Licensing

| | First year | After the first year, without a license | With a license |
|---|---|---|---|
| Run programs | any size | up to **1800 lines** | any size |
| Create `.exe` | yes | no | yes |

- The first year starts when you first run Freedom Basic.
- Lines are counted in the expanded program (the main file plus everything it loads with `$INCLUDE`), including blank lines and comments.
- Programs and `.exe` files **you** create belong entirely to you. You may distribute and sell them freely, with no royalties or other obligation.
- A license covers one user and one computer. Each extra computer of the same user gets a 30% discount.
- Planned licenses: **2 years, 30 EUR**, or **lifetime, 50 EUR**, valid for the major version you buy. They are not on sale yet; details will be announced here.

The full terms are a draft and are not final.

## Known limitations

- Freedom Basic is under active development. Differences from Liberty BASIC are possible; bug reports and short test programs that behave differently from Liberty BASIC are very welcome.

## Contact

Questions and bug reports: info@e-loukakis.gr
