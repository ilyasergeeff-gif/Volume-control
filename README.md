

{
   
  public partial class MainWindow : Window
  {
   public MainWindow()
         {
             InitializeComponent();
         }
   int a;
   string b;
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
