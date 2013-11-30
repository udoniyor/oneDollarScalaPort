oneDollarScalaPort
==================

A Scala version of the $1 Unistroke Recognizer originally created by  Wobbrock, J.O., Wilson, A.D. and Li, Y.  (dollar gesture recognizer) 
How to use this?

Add the code to your project. The code already includes number of gestures. In order to 
make of the recognizer you have to create one before hand:

	val myFirstRecognizer = recognizer()

Once you have a recognizer you can feed in more gestures or try to recognizer a gesture:

	//Adding a new Gesture:
	myFirstRecognizer.addGesture("circle",List(new Point(212,213).......

	//Recognizing Gestures:
	myFirstRecognizer.recognize(List(new Point(212,213).......

The recognizer returns a tumple with a message and a score:
	
	//Example of a returned tumple:
	("Circle", 6.23)
	or
	("No Match", 0.0)

You can enhance the recognizer further, by adding better control of the gestures and more.

