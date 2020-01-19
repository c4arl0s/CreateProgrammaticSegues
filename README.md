# CreateProgrammaticSegues
CreateProgrammaticSegues

# 1. Segues

Segues defines a transition from one view controller to another.

```swift
@IBOutlet weak var segueSwitch: UISwitch!
```

![Screen Recording 2020-01-18 at 22 05 59 2020-01-18 22_09_07](https://user-images.githubusercontent.com/24994818/72674690-32ed8900-3a3f-11ea-8667-d0b9562fdf3a.gif)

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

```swift
import UIKit

class ViewController: UIViewController {
    @IBOutlet weak var segueSwitch: UISwitch!
    
    override func viewDidLoad() {
        super.viewDidLoad()
        // Do any additional setup after loading the view, typically from a nib.
    }
    @IBAction func yellowButtonTapped(_ sender: Any) {
        if segueSwitch.isOn {
            performSegue(withIdentifier: "Yellow", sender: nil)
        }
    }
    @IBAction func greenButtonTapped(_ sender: Any) {
        if segueSwitch.isOn {
            performSegue(withIdentifier: "Green", sender: nil)
        }
    }
    
    override func didReceiveMemoryWarning() {
        super.didReceiveMemoryWarning()
        // Dispose of any resources that can be recreated.
    }


}
```


