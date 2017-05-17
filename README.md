package mergerGUI;

import java.awt.BorderLayout;
import java.awt.EventQueue;

import javax.swing.JFrame;
import javax.swing.JPanel;
import javax.swing.border.EmptyBorder;
import java.awt.FlowLayout;
import javax.swing.JButton;
import java.awt.GridLayout;
import java.awt.Color;
import javax.swing.JCheckBox;
import javax.swing.JProgressBar;
import javax.swing.JRadioButton;
import java.awt.event.ActionListener;
import java.awt.event.ActionEvent;
import javax.swing.JLabel;
import java.awt.GridBagLayout;
import java.awt.GridBagConstraints;
import java.awt.Insets;
import javax.swing.JEditorPane;
import javax.swing.JTextArea;
import javax.swing.JTabbedPane;
import javax.swing.JSplitPane;
import javax.swing.JToggleButton;
import javax.swing.JTextField;
import javax.swing.JList;
import javax.swing.JScrollBar;
import javax.swing.SwingConstants;
import javax.swing.DropMode;
import java.awt.Component;
import java.awt.Rectangle;
import java.awt.Dimension;
import javax.swing.JScrollPane;
import javax.swing.JComboBox;
import javax.swing.BoxLayout;
import javax.swing.Box;

public class mergerGUI extends JFrame {

	private JPanel contentPane;

	/**
	 * Launch the application.
	 */
	public static void main(String[] args) {
		EventQueue.invokeLater(new Runnable() {
			public void run() {
				try {
					mergerGUI frame = new mergerGUI();
					frame.setVisible(true);
				} catch (Exception e) {
					e.printStackTrace();
				}
			}
		});
	}

	/**
	 * Create the frame.
	 */
	public mergerGUI() {
		setBackground(Color.WHITE);
		setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
		setBounds(100, 100,800,600);
		contentPane = new JPanel();
		contentPane.setBorder(new EmptyBorder(5, 5, 5, 5));
		contentPane.setLayout(new BorderLayout(0, 0));
		setContentPane(contentPane);
		
		JPanel panel = new JPanel();
		contentPane.add(panel, BorderLayout.NORTH);
		panel.setLayout(new GridLayout(0, 3, 0, 0));
		
		JPanel panel_1 = new JPanel();
		panel.add(panel_1);
		panel_1.setLayout(new GridLayout(0, 3, 0, 0));
		
		JButton btnNewButton_5 = new JButton("load");
		panel_1.add(btnNewButton_5);
		
		JButton btnNewButton = new JButton("edit");
		panel_1.add(btnNewButton);
		
		JButton btnNewButton_3 = new JButton("save");
		panel_1.add(btnNewButton_3);
		
	
		JPanel panel_2 = new JPanel();
		panel.add(panel_2);
		
		JPanel panel_4 = new JPanel();
		panel.add(panel_4);
		panel_4.setLayout(new GridLayout(0, 3, 0, 0));
		
		JButton btnNewButton_1 = new JButton("load");
		panel_4.add(btnNewButton_1);
		
		JButton btnNewButton_2 = new JButton("edit");
		panel_4.add(btnNewButton_2);
		
		JButton btnNewButton_4 = new JButton("save");
		panel_4.add(btnNewButton_4);
		
		JTabbedPane tabbedPane = new JTabbedPane(JTabbedPane.TOP);
		contentPane.add(tabbedPane, BorderLayout.WEST);
		
		JTabbedPane tabbedPane_1 = new JTabbedPane(JTabbedPane.TOP);
		contentPane.add(tabbedPane_1, BorderLayout.EAST);
		
		JPanel panel_3 = new JPanel();
		contentPane.add(panel_3, BorderLayout.CENTER);
		panel_3.setLayout(new BoxLayout(panel_3, BoxLayout.X_AXIS));
		
		JTextArea textArea_1 = new JTextArea();
		panel_3.add(textArea_1);
		
		JScrollBar scrollBar = new JScrollBar();
		scrollBar.setSize(new Dimension(20, 0));
		panel_3.add(scrollBar);
	
		
		JPanel panel_5 = new JPanel();
		panel_5.setPreferredSize(new Dimension(14, 39));
		panel_3.add(panel_5);
		panel_5.setLayout(new BorderLayout(0, 0));
		
		JPanel panel_6 = new JPanel();
		panel_5.add(panel_6, BorderLayout.NORTH);
		panel_6.setLayout(new GridLayout(0, 1, 0, 0));
		
		JButton btnNewButton_6 = new JButton("compare");
		panel_6.add(btnNewButton_6);
		
		JPanel panel_7 = new JPanel();
		panel_5.add(panel_7, BorderLayout.CENTER);
		panel_7.setLayout(new GridLayout(1, 0, 0, 0));
		
		JButton btnNewButton_7 = new JButton("<-");
		panel_7.add(btnNewButton_7);
		
		JButton btnNewButton_8 = new JButton("->");
		panel_7.add(btnNewButton_8);
		
		JTextArea textArea = new JTextArea();
		panel_3.add(textArea);
		
		JScrollBar scrollBar_1 = new JScrollBar();
		scrollBar_1.setSize(new Dimension(20, 0));
		panel_3.add(scrollBar_1);
	}

}
