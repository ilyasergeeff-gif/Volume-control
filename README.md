
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
    numb = Convert.ToInt32(T1.Text);
    numb += 1;  
    wrd = Convert.ToString(numb);
    T1.Text = wrd;
    if (numb == 10)
     {
      B1.IsEnabled = false;
     }
     B2.IsEnabled = true;
    }
    

   private void B2_Click(object sender, RoutedEventArgs e)
    {
    numb = Convert.ToInt32(T1.Text);
    numb -= 1;
    b = Convert.ToString(numb);
    T1.Text = wrd;
    if (numb == 0)
     {
      B2.IsEnabled = false       
     }
     B1.IsEnabled = true;
    }
  }
 } 
