package com.example.calc;

import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.view.View;
import android.widget.EditText;
import android.widget.TextView;

public class MainActivity extends AppCompatActivity {

    private EditText editTextNumber1;
    private EditText editTextNumber2;
    private EditText editTextOperand;
    private TextView Answer;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        editTextNumber1 = findViewById(R.id.editTextnumber1);
        editTextNumber2 = findViewById(R.id.editTextnumber2);
        editTextOperand = findViewById(R.id.Operand);

        editTextNumber1.setShowSoftInputOnFocus(false);
        editTextNumber2.setShowSoftInputOnFocus(false);
        editTextOperand.setShowSoftInputOnFocus(false);

        Answer = findViewById(R.id.ansdisp);
    }

    private void updateNum1(String strToAdd) {
        String inp = editTextNumber1.getText().toString();
        editTextNumber1.setText(inp + strToAdd);
    }

    private void updateNum2(String strToAdd) {
        String inp2 = editTextNumber2.getText().toString();
        editTextNumber2.setText(inp2 + strToAdd);
    }

    private void updateOp(String strToAdd) {
        String inp3 = editTextOperand.getText().toString();
        editTextOperand.setText(inp3 + strToAdd);
    }

    public void equalBtn(View view) {
        String num1Str = editTextNumber1.getText().toString();
        String num2Str = editTextNumber2.getText().toString();
        String operandStr = editTextOperand.getText().toString();

        if (!num1Str.isEmpty() && !num2Str.isEmpty() && !operandStr.isEmpty()) {
            float num1 = Float.parseFloat(num1Str);
            float num2 = Float.parseFloat(num2Str);

            float result = 0;
            switch (operandStr) {
                case "+":
                    result = num1 + num2;
                    break;
                case "-":
                    result = num1 - num2;
                    break;
                case "x":
                    result = num1 * num2;
                    break;
                case "/":
                    if (num2 != 0) {
                        result = num1 / num2;
                    } else {
                        Answer.setText("Error: Division by zero");
                        return;
                    }
                    break;
                default:
                    Answer.setText("Error: Invalid operator");
                    return;
            }

            Answer.setText(String.valueOf(result));

        }
    }

    public void refreshBtn(View view) {
        editTextNumber1.setText("");
        editTextNumber2.setText("");
        editTextOperand.setText("");
        Answer.setText("");
    }

    public void zeroBtn(View view) {
        if (editTextNumber1.hasFocus()) {
            updateNum1("0");
        } else if (editTextNumber2.hasFocus()) {
            updateNum2("0");
        }
    }


    public void oneBtn(View view){
        if (editTextNumber1.hasFocus()) {
            updateNum1("1");
        } else if (editTextNumber2.hasFocus()) {
            updateNum2("1");

        }
    }
    public void twoBtn(View view){
        if (editTextNumber1.hasFocus()) {
            updateNum1("2");
        } else if (editTextNumber2.hasFocus()) {
            updateNum2("2");
        }
        }
    public void threeBtn(View view){
        if (editTextNumber1.hasFocus()) {
            updateNum1("3");
        } else if (editTextNumber2.hasFocus()) {
            updateNum2("3");
                }

    }
    public void fourBtn(View view){
        if (editTextNumber1.hasFocus()) {
            updateNum1("4");
        } else if (editTextNumber2.hasFocus()) {
            updateNum2("4");}


    }
    public void fiveBtn(View view){
        if (editTextNumber1.hasFocus()) {
            updateNum1("5");
        } else if (editTextNumber2.hasFocus()) {
            updateNum2("5");}

    }
    public void sixBtn(View view){
        if (editTextNumber1.hasFocus()) {
            updateNum1("6");
        } else if (editTextNumber2.hasFocus()) {
            updateNum2("6");}

    }
    public void sevenBtn(View view){
        if (editTextNumber1.hasFocus()) {
            updateNum1("7");
        } else if (editTextNumber2.hasFocus()) {
            updateNum2("7");}

    }
    public void eightBtn(View view){
        if (editTextNumber1.hasFocus()) {
            updateNum1("8");
        } else if (editTextNumber2.hasFocus()) {
            updateNum2("8");}

    }
    public void nineBtn(View view){
        if (editTextNumber1.hasFocus()) {
            updateNum1("9");
        } else if (editTextNumber2.hasFocus()) {
            updateNum2("9");}

    }

    public void multiplyBtn(View view) {
        updateOp("x");
    }

    public void addBtn(View view) {
        updateOp("+");
    }

    public void minusBtn(View view) {
        updateOp("-");
    }

    public void divideBtn(View view) {
        updateOp("/");
    }
}




