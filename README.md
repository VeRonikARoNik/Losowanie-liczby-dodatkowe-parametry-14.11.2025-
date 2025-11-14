
# Losowanie-liczby-dodatkowe-parametry-14.11.2025
# I

<img width="906" height="532" alt="image" src="https://github.com/user-attachments/assets/763fdeac-45a2-4c3e-bdec-576010cd2724" />

```
using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace Losowanie_liczby
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
        }

        private void button1_Click(object sender, EventArgs e)
        {

            Random rng = new Random();

            int from, to;

            if (int.TryParse(textBox1.Text, out from) &&
                int.TryParse(textBox2.Text, out to) &&
                from <= to)
            {
                int number = rng.Next(from, to + 1);
                label1.Text = "Wylosowano: " + number;
            }
            else
            {
                label1.Text = "Błędne dane!";
            }
        }

        private void label1_Click(object sender, EventArgs e)
        {

        }
    }
}

```


# II


# Dodaj liczbę losowań liczb

<img width="919" height="520" alt="image" src="https://github.com/user-attachments/assets/00c4abb3-8ab2-4736-ab8d-9a0c19f87ec3" />

```

            Random rng = new Random();

            int from, to, count;

            if (int.TryParse(textBox1.Text, out from) &&
                int.TryParse(textBox2.Text, out to) &&
                int.TryParse(textBox3.Text, out count) &&
                from <= to &&
                count > 0)
            {
                listBox1.Items.Clear(); // czyścimy poprzednie wyniki

                for (int i = 0; i < count; i++)
                {
                    int number = rng.Next(from, to + 1);
                    listBox1.Items.Add(number);
                }
            }
            else
            {
                MessageBox.Show("Błędne dane wejściowe!");
            }

```

# III

# Dodaj losowanie bez powturzeń 


# IV

# Dodaj  dwa radiobutton parzyste i nieparzyste losowanie


Wykonaj zrzut ekranu wykonanych zadań opisz dokumencie word

e-mail: 
wykonanezadania100@gmail.com



