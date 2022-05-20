# Ejercicio-2
El c# con orientación a objetos realiza un aplicativo similar a la calculadora de Windows

namespace Calculadora
{
    public partial class Form1 : Form
    {
        private double valor1;
        private double valor2;
        private double resultado;
        private int operacion;

        public Form1()
        {
            InitializeComponent();
        }

        private void textBox1_TextChanged(object sender, EventArgs e)
        {
        }

        private void bt0_Click(object sender, EventArgs e)
        {
            //numero 0
            tablero.Text = tablero.Text + "0";
        }

        private void bt1_Click(object sender, EventArgs e)
        {
            //numero 1
            tablero.Text = tablero.Text + "1";
        }

        private void bt2_Click(object sender, EventArgs e)
        {
            //numero 2
            tablero.Text = tablero.Text + "2";
        }

        private void bt3_Click(object sender, EventArgs e)
        {
            //numero 3
            tablero.Text = tablero.Text + "3";
        }

        private void bt4_Click(object sender, EventArgs e)
        {
            //numero 4
            tablero.Text = tablero.Text + "4";
        }

        private void bt5_Click(object sender, EventArgs e)
        {
            //numero 5
            tablero.Text = tablero.Text + "5";
        }

        private void bt6_Click(object sender, EventArgs e)
        {
            //numero 6
            tablero.Text = tablero.Text + "6";
        }

        private void bt7_Click(object sender, EventArgs e)
        {
            //numero 7
            tablero.Text = tablero.Text + "7";
        }

        private void bt8_Click(object sender, EventArgs e)
        {
            //numero 8
            tablero.Text = tablero.Text + "8";
        }

        private void bt9_Click(object sender, EventArgs e)
        {
            //numero 9
            tablero.Text = tablero.Text + "9";
        }

        private void btLimpiar_Click(object sender, EventArgs e)
        {
            //boton limpiar
            tablero.Text = "";
        }

        private void btIgual_Click(object sender, EventArgs e)
        {
            //boton igual
            valor2 = Convert.ToDouble(tablero.Text);
            switch (operacion)
            {
                case 1:
                    resultado = valor1 + valor2;
                    break;
                case 2:
                    resultado = valor1 - valor2;
                    break;
                case 3:
                    resultado = valor1 * valor2;
                    break;
                case 4:
                    resultado = valor1 / valor2;
                    break;
            }
            tablero.Text = resultado.ToString();
        }

        private void btSuma_Click(object sender, EventArgs e)
        {
            //boton suma
            operacion = 1;
            valor1 = Convert.ToDouble(tablero.Text);
            tablero.Text = "";
        }

        private void btResta_Click(object sender, EventArgs e)
        {
            //boton resta
            operacion = 2;
            valor1 = Convert.ToDouble(tablero.Text);
            tablero.Text = "";
        }
        private void btMultiplicacion_Click(object sender, EventArgs e)
        {
            //boton multiplicacion
            operacion = 3;
            valor1 = Convert.ToDouble(tablero.Text);
            tablero.Text = "";
        }
        private void btDivision_Click(object sender, EventArgs e)
        {
            //boton division
            operacion = 4;
            valor1 = Convert.ToDouble(tablero.Text);
            tablero.Text = "";
        }

        private void btPunto_Click(object sender, EventArgs e)
        {
            //boton punto
            tablero.Text = tablero.Text + ".";
        }

    }
}
