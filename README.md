<img src="https://github.com/anhvu1993/PDFZoomKit/blob/main/PDFZoomKit/ScreenShot.jpeg" alt="" />
# PDFZoomKit
PDFZoomKit is a Swift framework a simple zoom tool that supports professional image enlargement

## Requirements

- iOS 13.0+
- Xcode 12.0+
- Swift 4.0+

## Installation

### CocoaPods
[CocoaPods](http://cocoapods.org) is a dependency manager for Cocoa projects. You can install it with the following command:

To integrate PDFZoomKit into your Xcode project using CocoaPods, specify it in your `Podfile`:
```
pod 'PDFZoomKit'
```
or
```
pod 'PDFZoomKit', :git => "https://github.com/anhvu1993/PDFZoomKit.git", :tag => '0.0.4'
```
Then, run the following command:

```bash
$ pod install
```

## Usage

### Quick Start

```swift
import PDFZoomKit

class MyViewController: UIViewController {

    private var toolZoom: ToolZoomManager!

    override func viewDidLoad() {
        super.viewDidLoad()
        toolZoom = ToolZoomManager(viewPDF: pdfView, mainView: self.view, strokeColor: UIColor.red.cgColor)
    }
    
    func show() {
      toolZoom.showToolZoom(isShow: true) // True or false
    }

}
```
## License

PDFZoomKit is released under the MIT license. See LICENSE for details.
