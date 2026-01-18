# QSL Card Designer (QSLカードデザイナー)

A web-based tool for amateur radio operators to design and create custom QSL cards with ADIF log file support.

アマチュア無線運用者がADIFログファイルを使用してカスタムQSLカードをデザイン・作成するためのWebベースツールです。

## Demo (デモ)

**Live Demo**: https://www.shvtech.com/radio/QSL_card_designer/

## Screenshots (スクリーンショット)

<!-- TODO: Add screenshots here -->
<!-- Add a screenshot of the main interface showing:
     1. The sidebar with ADIF import and field management
     2. The designer area with positioned fields
     3. A completed QSL card design with background image

Example:
![QSL Card Designer Interface](screenshots/main-interface.png)
![Sample QSL Card](screenshots/sample-card.png)
-->

_Screenshots coming soon! Please add screenshots showing the interface and sample QSL cards._

_スクリーンショット準備中！インターフェースとサンプルQSLカードのスクリーンショットを追加してください。_

## Features (機能)

### Core Features (主要機能)
- **ADIF Import** (ADIFインポート): Import standard ADIF (.adi, .adif) log files containing radio contact records
- **Visual Designer** (ビジュアルデザイナー): Drag-and-drop interface for positioning fields on your QSL card
- **Field Management** (フィールド管理): Add, position, resize, and customize any ADIF field
- **Background Images** (背景画像): Upload custom background images for your QSL cards
- **Font & Color Customization** (フォント・カラーカスタマイズ): Customize fonts and colors for callsign fields
  - 30 font options available
  - 15-color palette plus custom color picker
- **PNG Export** (PNG出力): Download your designed cards as high-quality PNG images
- **Multi-QSO Support** (複数QSO対応): Switch between different QSO records from your log file

### Supported Fields (対応フィールド)
- Station Callsign (無線局コールサイン)
- QSO Date (交信日)
- Start Time (開始時刻)
- Band (バンド)
- Frequency (周波数)
- Mode (モード)
- Operator (運用者)
- Other Station Callsign (相手局)
- RST Sent/Received (送信/受信RST)
- Grid Locator (グリッドロケーター)
- Name (相手氏名)
- QTH/Location (相手住所/地域)
- And any other fields in your ADIF file

## What is a QSL Card? (QSLカードとは？)

QSL cards are written confirmation cards used by amateur radio operators to confirm radio contact (QSO) between two stations. Traditionally, these cards are exchanged by mail and serve as proof of communication. They often feature custom designs, station information, and contact details.

QSLカードは、アマチュア無線運用者が2局間の無線交信（QSO）を確認するために使用する書面による確認カードです。伝統的に、これらのカードは郵便で交換され、通信の証拠として機能します。カスタムデザイン、局情報、交信詳細が記載されることが多いです。

## Getting Started (使い方)

### Requirements (必要要件)
- Modern web browser (Chrome, Firefox, Safari, Edge)
- No installation required - runs entirely in your browser
- No server needed - all processing is client-side

### How to Use (使用方法)

1. **Open the Application** (アプリケーションを開く)
   - Simply open `QSL_card_designer.html` in your web browser
   - Or visit the live demo: https://www.shvtech.com/radio/QSL_card_designer/

2. **Import Your ADIF Log** (ADIFログをインポート)
   - Click "Import ADIF File (ADIFファイルをインポート)"
   - Select your .adi or .adif log file
   - Your QSO records will be loaded automatically

3. **Select a QSO** (QSOを選択)
   - Use the "Select QSO (QSO選択)" dropdown to choose which contact to design a card for
   - The preview will update automatically

4. **Add Background Image** (Optional) (背景画像を追加)
   - Click "QSL Card Background Image (QSLカード背景画像)"
   - Upload your custom background image (JPG, PNG, etc.)
   - The image will auto-scale to fit while maintaining aspect ratio

5. **Add Fields** (フィールドを追加)
   - Select a field from "Add New Field (新しいフィールドを追加)" dropdown
   - Click "Add (追加)" button
   - The field will appear on the card

6. **Position and Resize Fields** (フィールドの配置とリサイズ)
   - **Move**: Click and drag any field to reposition it
   - **Resize**: Click and drag the small handle in the bottom-right corner of each field
   - **Toggle Field Name**: Click "Name (名前) ON/OFF" to show/hide the field label

7. **Customize Fonts and Colors** (フォントと色のカスタマイズ) (For Station/Call fields)
   - Click "Style (スタイル)" button on STATION_CALLSIGN or CALL fields
   - Choose from 30 different fonts
   - Select a color from the palette or use the custom color picker

8. **Download Your Card** (カードをダウンロード)
   - Click "Download as PNG (PNGとしてダウンロード)"
   - Your QSL card will be saved as a PNG image file

9. **Create More Cards** (さらにカードを作成)
   - Select a different QSO from the dropdown
   - The same design will be applied with different contact data
   - Download each card individually

## Technology Stack (技術スタック)

- **HTML5**: Structure and layout
- **CSS3**: Styling and visual design
- **Vanilla JavaScript**: All functionality (no frameworks or dependencies)
- **HTML5 Canvas API**: PNG export functionality
- **FileReader API**: Client-side file processing

## Browser Compatibility (ブラウザ互換性)

Tested and working on:
- Google Chrome (recommended)
- Mozilla Firefox
- Safari
- Microsoft Edge

Requires a modern browser with support for:
- FileReader API
- HTML5 Canvas
- CSS3 Flexbox
- ES6 JavaScript

## Privacy (プライバシー)

All processing happens entirely in your browser. Your ADIF files and QSL card designs:
- Are NEVER uploaded to any server
- Stay completely private on your computer
- Are processed locally using client-side JavaScript

すべての処理はブラウザ内で完結します。ADIFファイルとQSLカードデザイン：
- サーバーにアップロードされることはありません
- 完全にプライベートでコンピューター内に保持されます
- クライアントサイドのJavaScriptを使用してローカルで処理されます

## File Structure (ファイル構成)

```
QSL-Card-Designer/
├── QSL_card_designer.html    # Main application file (single-file application)
├── README.md                   # This file
└── LICENSE                     # Apache License 2.0
```

## Contributing (貢献)

Contributions are welcome! This is a simple single-file application, making it easy to contribute.

To contribute:
1. Fork the repository
2. Make your changes to `QSL_card_designer.html`
3. Test thoroughly in multiple browsers
4. Submit a pull request

## Future Enhancements (今後の改善予定)

Potential features for future development:
- Save/Load design templates
- Batch export for all QSOs
- Print functionality
- More field customization options (fonts/colors for all fields)
- Multi-language UI switching
- Template gallery
- Support for more ADIF fields

## License (ライセンス)

This project is licensed under the Apache License 2.0 - see the LICENSE file for details.

## Credits (クレジット)

Developed with assistance from [Cursor AI](https://github.com/cursor/cursor)

## Support (サポート)

For issues, questions, or suggestions, please open an issue on GitHub.

---

**73!** (Amateur radio sign-off meaning "best regards")

**ハムライフを楽しんでください！** (Enjoy your ham radio life!)
