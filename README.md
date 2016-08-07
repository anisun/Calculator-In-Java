
package test;

import javax.swing.JButton;
import javax.swing.JFrame;
import javax.swing.JTextField;

public class JavaCalculator {

    JFrame jf;
   //JPanel jp = new JPanel();
    JTextField jtf;
    JButton b1, b2, b3, b4, b5, b6, b7, b8, b9, b0, badd, bsub, bmul, bdiv, bclear, bdel, beq, bdot;
    static double a=0,b=0,result=0;
    static int operator=0;
    public int len=0;
    

    public JavaCalculator() {
        this.jf = new JFrame("Calculator");
        jtf = new JTextField();
        jf.setSize(300, 400);
        jf.setLocation(45, 45);
        b0 = new JButton("0");
        b1 = new JButton("1");
        b2 = new JButton("2");
        b3 = new JButton("3");
        b4 = new JButton("4");
        b5 = new JButton("5");
        b6 = new JButton("6");
        b7 = new JButton("7");
        b8 = new JButton("8");
        b9 = new JButton("9");
        badd = new JButton("+");
        bsub = new JButton("-");
        bmul = new JButton("x");
        bdiv = new JButton("/");
        bclear = new JButton("Clear");
        bdel = new JButton("D");
        beq = new JButton("=");
        bdot = new JButton(".");

        jtf.setBounds(25, 10, 230, 30);
        bclear.setBounds(10, 60, 120, 40);
        bdel.setBounds(150, 60, 50, 40);
        bdiv.setBounds(220, 60, 50, 40);

        b7.setBounds(10, 120, 50, 40);
        b8.setBounds(80, 120, 50, 40);
        b9.setBounds(150, 120, 50, 40);
        bmul.setBounds(220, 120, 50, 40);

        b4.setBounds(10, 180, 50, 40);
        b5.setBounds(80, 180, 50, 40);
        b6.setBounds(150, 180, 50, 40);
        bsub.setBounds(220, 180, 50, 40);

        b1.setBounds(10, 240, 50, 40);
        b2.setBounds(80, 240, 50, 40);
        b3.setBounds(150, 240, 50, 40);
        badd.setBounds(220, 240, 50, 40);

        b0.setBounds(10, 300, 50, 40);
        bdot.setBounds(80, 300, 50, 40);
        beq.setBounds(150, 300, 100, 40);

        jf.add(jtf);
        jf.add(bclear);
        jf.add(bdel);
        jf.add(bdiv);
        jf.add(b7);
        jf.add(b8);
        jf.add(b9);
        jf.add(bmul);
        jf.add(b0);
        jf.add(b1);
        jf.add(b2);
        jf.add(b3);
        jf.add(b4);
        jf.add(b5);
        jf.add(b6);
        jf.add(badd);
        jf.add(bsub);
        jf.add(bdot);
        jf.add(beq);

        jf.setLayout(null);
        jf.setVisible(true);
        jf.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
        jf.setResizable(false);
        
        b1.addActionListener(this::b1ActionPerformed);
        b2.addActionListener(this::b2ActionPerformed);
        b3.addActionListener(this::b3ActionPerformed);
        b4.addActionListener(this::b4ActionPerformed);
        b5.addActionListener(this::b5ActionPerformed);
        b6.addActionListener(this::b6ActionPerformed);
        b7.addActionListener(this::b7ActionPerformed);
        b8.addActionListener(this::b8ActionPerformed);
        b9.addActionListener(this::b9ActionPerformed);
        b0.addActionListener(this::b0ActionPerformed);
        badd.addActionListener(this::baddActionPerformed);
        bdiv.addActionListener(this::bdivActionPerformed);
        bmul.addActionListener(this::bmulActionPerformed);
        bsub.addActionListener(this::bsubActionPerformed);
        bdot.addActionListener(this::bdotActionPerformed);
        beq.addActionListener(this::beqActionPerformed);
        bdel.addActionListener(this::bdelActionPerformed);
        bclear.addActionListener(this::bclearActionPerformed);
    }
    
    private void b1ActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here:
        String s1 = b1.getText();
        String s2 = jtf.getText();
        String s = s2 + s1;
        jtf.setText(s);
    }  
    
    private void b2ActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here:
        String s1 = b2.getText();
        String s2 = jtf.getText();
        String s = s2 + s1;
        jtf.setText(s);
    } 
    
    private void b3ActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here:
        String s1 = b3.getText();
        String s2 = jtf.getText();
        String s = s2 + s1;
        jtf.setText(s);
    } 
    
    private void b4ActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here:
        String s1 = b4.getText();
        String s2 = jtf.getText();
        String s = s2 + s1;
        jtf.setText(s);
    } 
    
    private void b5ActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here:
        String s1 = b5.getText();
        String s2 = jtf.getText();
        String s = s2 + s1;
        jtf.setText(s);
    } 
    
    private void b6ActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here:
        String s1 = b6.getText();
        String s2 = jtf.getText();
        String s = s2 + s1;
        jtf.setText(s);
    } 
    
    private void b7ActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here:
        String s1 = b7.getText();
        String s2 = jtf.getText();
        String s = s2 + s1;
        jtf.setText(s);
    } 
    
    private void b8ActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here:
        String s1 = b8.getText();
        String s2 = jtf.getText();
        String s = s2 + s1;
        jtf.setText(s);
    } 
    
    private void b9ActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here:
        String s1 = b9.getText();
        String s2 = jtf.getText();
        String s = s2 + s1;
        jtf.setText(s);
    } 
    
    private void b0ActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here:
        String s1 = b0.getText();
        String s2 = jtf.getText();
        String s = s2 + s1;
        jtf.setText(s);
    } 
    
    private void baddActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here:
        String s1 = badd.getText();
        String s2 = jtf.getText();
        String s = s2 + s1;
        jtf.setText(s);
    } 
    
    private void bsubActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here:
        String s1 = bsub.getText();
        String s2 = jtf.getText();
        String s = s2 + s1;
        jtf.setText(s);
    } 
    
    private void bmulActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here:
        String s1 = bmul.getText();
        String s2 = jtf.getText();
        String s = s2 + s1;
        jtf.setText(s);
    } 
    
    private void bdivActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here:
        String s1 = bdiv.getText();
        String s2 = jtf.getText();
        String s = s2 + s1;
        jtf.setText(s);
    } 
    
    private void bdotActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here:
        String s1 = bdot.getText();
        String s2 = jtf.getText();
        String s = s2 + s1;
        jtf.setText(s);
    } 
    
    private void beqActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here:
        String s1 = jtf.getText();
        int len = s1.length();
        char c;
        char ch = 0;
        int len1 = 0;
        
        for(int i = 0; i < len; i++) {
            c = s1.charAt(i);
            if((c != '+') && (c != '-') && (c != 'x') && (c != '/')) {
                len1++;
            }
            else {
                ch = c;
                break;
            }
        }
        
        //System.out.println("Hello World! = " + len1 + " and " + len);
        String s2 = "";
        //char c2;
        
        for(int j = 0; j < len1; j++) {
            char c2 = s1.charAt(j);
            s2 += c2;
        }
        
        //int lll = s2.length();
         //System.out.println("Hello World! = " + lll);
        //System.out.println("Hello World!");
        String s3 = "";
        //char c3;
        
        for(int k = len1+1; k < len; k++) {
            char c3 = s1.charAt(k);
            s3  = s3 + c3;
        }

         //System.out.println("Hello World!");
         
        long a = Long.parseLong(s2);
        long b = Long.parseLong(s3);
        long d = 0;
        
        if(ch == '+') {
            d = a + b;
        }
        else if(ch == '-') {
            d = a - b;
        }
        
        else if(ch == 'x') {
            d = a * b;
        }
        
        else if(ch == '/') {
            d = a / b;
        }
        
        String s = String.valueOf(d);
        
        jtf.setText(s);
    } 
    
    private void bclearActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here:
        String s = "";
        jtf.setText(s);
    } 
    
    private void bdelActionPerformed(java.awt.event.ActionEvent evt) {                                         
        // TODO add your handling code here:
        String s1 = jtf.getText();
        int l = s1.length();
        char c;
        String s = "";
        for(int i = 0; i < l-1; i++) {
            c = s1.charAt(i);
            s += c;
        }
        jtf.setText(s);
    } 

    public static void main(String[] args) {
        JavaCalculator javacal = new JavaCalculator();
    }
}
