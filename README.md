# GestureRecognizer

A gesture recognizer is an object that will listen for the user to input a common gesture and will call an action when the particular gesture is recognized.

A gesture is tied to a single view, but a view can have multiple gestures.

``` swift
//
//  ViewController.swift
//  GestureRecognizer
//
//  Created by Carlos Santiago Cruz on 23/08/18.
//  Copyright © 2018 Carlos Santiago Cruz. All rights reserved.
//

import UIKit

class ViewController: UIViewController {

    override func viewDidLoad() {
        super.viewDidLoad()
        // Do any additional setup after loading the view, typically from a nib.
    }
    @IBAction func tapGestureOcurred(_ sender: UITapGestureRecognizer) {
        let location = sender.location(in: view)
        print(location)
        // it prints the coordinates where you tapped on screen. Look at the console
        // no necesita de un outlet, preguntar por qué ?

    }
    

    override func didReceiveMemoryWarning() {
        super.didReceiveMemoryWarning()
        // Dispose of any resources that can be recreated.
    }


}
```

