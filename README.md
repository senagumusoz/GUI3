# GUI3
ex3
import javax.swing.ImageIcon;
import javax.swing.JButton;
import javax.swing.JFrame;
import javax.swing.JPanel;
import javax.swing.SwingConstants;

public class GUI4 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub

		JFrame.setDefaultLookAndFeelDecorated(true);//çerceve şekli
		JFrame frame=new JFrame("GUI Çalışıyoruz!!");
		
		JPanel GUI=new JPanel();
		GUI.setLayout(null);
		
		JPanel dugmeler=new JPanel();
		dugmeler.setLocation(10,10);
		dugmeler.setSize(250,275);
		GUI.add(dugmeler);
		
		JButton jb1=new JButton();
		jb1.setText("buna basma");
	    jb1.setSize(120,20);
	    jb1.setLocation(70,20);
	    jb1.setHorizontalAlignment(0);
	    dugmeler.add(jb1);
	    
	    frame.setSize(290,300);
	    frame.setContentPane(GUI);
	    frame.setResizable(false);
	    frame.setVisible(true);
	    
	    JButton jb2=new JButton();
	    jb2.setText("buna bas");
	    jb2.setSize(120,20);
	    jb2.setLocation(70,45);
	    jb2.setHorizontalAlignment(4);
	    dugmeler.add(jb2);
		
	    ImageIcon ıc1=new ImageIcon("C:/Users/sena/OneDrive/Masaüstü/DERSLER/Nesneye Yönelik Programlama/cup.jpg");
	    JButton jb3=new JButton(ıc1);
	    jb3.setSize(110,70);
	    jb3.setLocation(75,75);
	    jb3.setHorizontalAlignment(0);
	    dugmeler.add(jb3);
		
	    
	  
	    JButton jb4=new JButton("sağ",ıc1);
	    jb4.setSize(110,170);
	    jb4.setLocation(10,155);	    
	    dugmeler.add(jb4);
	    
	   
	    JButton jb5=new JButton("sol",ıc1);
	    jb5.setSize(110,70);
	    jb5.setLocation(130,155);
	   jb5.setHorizontalTextPosition(SwingConstants.LEFT);
	    dugmeler.add(jb5);
	}

}
