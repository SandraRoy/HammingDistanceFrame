# Project5
**_public class HammingDistanceFrame_**
The class implements ChangeListener and ActionListener in order to implememnt any changes through the JComponents. First appproach was to create the front end using GUI componenets and I derived my back end(logic) from Project 1 in 
order to find the Hamming Distance.

**_public HammingDistnaceFrame()_**
 In order to set up the sliders, I declared and initialized a min value, a max value and used the majorTickSpacing method to assign the metric 
 points on the slider. I also added it to ChangeListener in order for it to respond to the change made by the user. 
 
 I declared and Initialized THe various JTextFields and JTextAreas, set their size, and visibility.
 I also declared and initialized labels and set the text.
 For the buttons, after declaration and initialization, I added to it to ActionListener in order to implement the 
 actions required by the button.
 I mainly used GridBagLayout to set up the different JComponents
 I set up the Enter Distance label at coordinate (0,0) using gridx and gridy to set up the points. I declared a GridBagConstraints variable and 
 used it call the anchor method in order to determine the alignment of the component using LINE_END, LINE_START, HORIZONTAL. 
 I used gridwidth to set size and the **insets** method which determines the spacing around the top, left, bottom, and right of the element.
 
 **_public void stateChanged()_**
 
 This method takes a ChangeEvent variable as parameter and checks for a slider to be the source of the event. If the condition is fulfilled, it
 displays the value on the slider to its corresponding text box.
 
 **_public int findDistance_**
 This method takes to string variables and finds the Hamming Distance between them. It loops through each character of both words and updates a 
 count variale for eery difference in character.
 
 **_public int[] numberNodes_**
 This method counts the number of nodes from a given word in the parameter. It returns an array with a count variable for number of nodes for each
 possible distance form the word.
 
 **_public void read()_**
 This method reads in Mesonet.txt into an ArrayList of words.
 
 
**_public static void main()_**
Creates a HammingDistanceFrame object in order to display it.

**_public void actionPerformed_**
This method must be implemented by the class as it implements ActionListener. If the event source is the Show Distance button, it calls
the findDistance methods and displays the words that have a HammingDistance specified by the slider compared to the item Selected from the JComboBox

If the event source is Calculate HD it calls the numberNodes method and displays each possible distance for the item selected from the MEnu box.
If the event source is the Add Station method, It adds the word in the text box entered by he use to the JComboBox
It also checks event sources in the JRadioButtons and displays a corresponding message accoring to the user's choice.

My creative portion lets the user rate the program and has a short mood questionnaire.

 
 
