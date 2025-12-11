using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows;
using System.Windows.Controls;
using System.Windows.Data;
using System.Windows.Documents;
using System.Windows.Input;
using System.Windows.Media;
using System.Windows.Media.Imaging;
using System.Windows.Navigation;
using System.Windows.Shapes;
namespace WpfApp1
{
    /// <summary>
    /// Логика взаимодействия для MainWindow.xaml
    /// </summary>
  public partial class MainWindow : Window
  {
   public MainWindow()
         {
             InitializeComponent();
         }
   int numb;
   string wrd;
   private void B1_Click(object sender, RoutedEventArgs e)
   {
    a = Convert.ToInt32(T1.Text);
    a += 1;  
    b = Convert.ToString(a);
    T1.Text = b;
    if (a == 10)
     {
      B1.IsEnabled = false;
     }
     B2.IsEnabled = true;
    }
    

   private void B2_Click(object sender, RoutedEventArgs e)
    {
    a = Convert.ToInt32(T1.Text);
    a -= 1;
    b = Convert.ToString(a);
    T1.Text = b;
    if (a == 0)
     {
      B2.IsEnabled = false       
     }
     B1.IsEnabled = true;
    }
  }
 } 
