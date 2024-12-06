import java.util.*;
import java.awt.event.*; // For action events
// Inheriting JFrame class
public class ButtonWithInheritance extends JFrame {
    // Constructor to set up the JFrame and add components
    public ButtonWithInheritance() {
        setTitle("Swing Button with Inheritance");
        setLayout(null);
        JButton button = new JButton("Click Me!");
        button.setBounds(100, 100, 120, 40);
        add(button);
        button.addActionListener(new ActionListener() {
            @Override
            public void actionPerformed(ActionEvent e) {
                 JOptionPane.showMessageDialog(null, "Button Clicked!");
            }
        });
        setSize(400, 300);
        setVisible(true);
        setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
    }
    public static void main(String[] args) {
        // Directly invoking the constructor to create an instance of the class
        new ButtonWithInheritance();
    }
}
{
    public static void main (String[] args)
    {
        System.out.println("the num of arguments placed are"+ args.length);
        for(int i=0;i<=args.length;i++)
        {
            System.out.println("the arguments in array [i] is"+args[i]);
        }
    }
    
}
