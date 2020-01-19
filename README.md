# CreateProgrammaticSegues
CreateProgrammaticSegues

# 1. Segues

Segues defines a transition from one view controller to another.

```swift
@IBOutlet weak var segueSwitch: UISwitch!
```

![Screen Shot 2020-01-18 at 22 01 34](https://user-images.githubusercontent.com/24994818/72674596-27e62900-3a3e-11ea-8aa3-0c1dd454a882.png)

# 2. Create an action for each button

```swift
@IBAction func yellowButtonTapped(_ sender: Any) {
        if segueSwitch.isOn{
            performSegue(withIdentifier: "Yellow", sender: nil)
        }
    }
```

```swift
@IBAction func greenButtonTapped(_ sender: Any) {
        if segueSwitch.isOn {
            performSegue(withIdentifier: "Green", sender: nil)
        }
    }
```
