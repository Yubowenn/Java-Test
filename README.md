import javax.swing.*;
import java.awt.*;
//import java.awt.event.*;

class Test extends JFrame //implements ActionListener,ItemListener
{
	JTextField jt=new JTextField(30);
	Test()
	{
		setSize(300,300);
		setVisible(true);
		setTitle("report");
		setLayout(new BorderLayout());
		Container c= getContentPane();
		//设置窗体信息

		JPanel p1=new JPanel();
		JPanel p2=new JPanel();
		JPanel p3=new JPanel();

		JLabel jlb1=new JLabel("Age:");
		JLabel jlb2=new JLabel("Hobbies:");
		JLabel jlb3=new JLabel("Result:");
		//创建标签信息

		JRadioButton jrt1=new JRadioButton("5~15");
		JRadioButton jrt2=new JRadioButton("16~25");
		JRadioButton jrt3=new JRadioButton("26~35");
		JRadioButton jrt4=new JRadioButton("36~45");
		JRadioButton jrt5=new JRadioButton("46~55");


		JCheckBox cb1=new JCheckBox("chating");
		JCheckBox cb2=new JCheckBox("sports");
		JCheckBox cb3=new JCheckBox("shopping");
		JCheckBox cb4=new JCheckBox("vacation");
		JCheckBox cb5=new JCheckBox("clothes");


		JButton jbt1=new JButton("Comfirm");
		JButton jbt2=new JButton("Remove");

		//jrt1.addActionListen(this);
		add(jrt1);
		//jrt2.addActionListen(this);
		add(jrt2);
		//jrt3.addActionListen(this);
		add(jrt3);
		//jrt4.addActionListen(this);
		add(jrt4);
		//jrt5.addActionListen(this);
		add(jrt5);

		//cb1.addItemListener(this);
		add(cb1);
		//cb2.addItemListener(this);
		add(cb2);
		//cb3.addItemListener(this);
		add(cb3);
		//cb4.addItemListener(this);
		add(cb4);
		//cb5.addItemListener(this);
		add(cb5);


		ButtonGroup bg=new ButtonGroup();
		bg.add(jrt1);
		bg.add(jrt2);
		bg.add(jrt3);
		bg.add(jrt4);
		bg.add(jrt5);


		p1.add(jlb1);
		p1.add(jrt1);
		p1.add(jrt2);
		p1.add(jrt3);
		p1.add(jrt4);
		p1.add(jrt5);
		//p1面板
		p2.add(jlb2);
		p2.add(cb1);
		p2.add(cb2);
		p2.add(cb3);
		p2.add(cb4);
		p2.add(cb5);
		//p2面板
		p3.add(jlb3);
		p3.add(jt);
		p3.add(jbt1);
		p3.add(jbt2);
		//p3面板

		c.add("North",p1);
		c.add("Center",p2);
		c.add("South",p3);
		

		validate();
		setDefaultCloseOperation(EXIT_ON_CLOSE);
	}
}

public class GUIExample
{
	public static void main(String[] args)
	{
		Test t=new Test();
	}
}
