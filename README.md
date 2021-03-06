# Untagger

Untagger is a removal and full text extraction of HTML written in Swift heavily inspired by <a href="https://github.com/kohlschutter/boilerpipe">Boilerpipe</a>.

<img src="https://github.com/wcgray/Untagger/blob/master/demo.gif" width="440" height="868" /></a>

## Installation

Use CocoaPods:

```ruby
pod 'Untagger', '~> 0.0.1'
```

Or drag the Untagger project into your xcodeproj and make Untagger a target dependency.

## Usage

```swift
UntaggerManager.sharedInstance.getText(url: url) { (title, body, source, error) in
            if error == nil {
                print("Article title: \(title!)")
                print("Article body: \(body!)")
            }

            if let error = error {
                print("Error: \(error.message)")
            }
        }
```

## License

MIT
