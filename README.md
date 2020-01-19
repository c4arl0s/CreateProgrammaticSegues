# CreateProgrammaticSegues
CreateProgrammaticSegues

# 1. Segues

Segues defines a transition from one view controller to another.

```swift
@IBOutlet weak var segueSwitch: UISwitch!
```

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
