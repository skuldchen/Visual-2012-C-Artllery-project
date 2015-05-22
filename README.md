# Visual-2012-C-sharp-Artllery-code
No comment.
-----------------------------------------------------------------------
<Page
    x:Class="App002.MainPage"
    xmlns="http://schemas.microsoft.com/winfx/2006/xaml/presentation"
    xmlns:x="http://schemas.microsoft.com/winfx/2006/xaml"
    xmlns:local="using:App002"
    xmlns:d="http://schemas.microsoft.com/expression/blend/2008"
    xmlns:mc="http://schemas.openxmlformats.org/markup-compatibility/2006"
    mc:Ignorable="d">

    <Grid RenderTransformOrigin="0.411,0.412" AllowDrop="True">
        <Grid.Background>
            <LinearGradientBrush EndPoint="0.5,1" StartPoint="0.5,0">
                <GradientStop Color="Black"/>
                <GradientStop Color="#FFE6ADFB" Offset="1"/>
            </LinearGradientBrush>
        </Grid.Background>
        <Grid.ColumnDefinitions>
            <ColumnDefinition/>
        </Grid.ColumnDefinitions>
        <Button Content="Cal Distance" HorizontalAlignment="Left" Margin="213,386,0,0" VerticalAlignment="Top" Click="Button_Click_1" Height="38" Width="121"/>
        <Button x:Name="btnFirToTar" Content="Fir To Tar" HorizontalAlignment="Left" Margin="583,386,0,0" VerticalAlignment="Top" Height="38" Width="94" Click="btnFirToTar_Click"/>
        <TextBlock HorizontalAlignment="Left" Margin="60,149,0,0" TextWrapping="Wrap" Text="FireNlat" VerticalAlignment="Top" Height="13" Width="127" FontSize="14"/>
        <TextBlock HorizontalAlignment="Left" Margin="60,186,0,0" TextWrapping="Wrap" Text="FireElong" VerticalAlignment="Top" Height="13" Width="127" FontSize="14"/>
        <TextBox x:Name="textBox1" HorizontalAlignment="Left" Margin="213,130,0,0" TextWrapping="Wrap" VerticalAlignment="Top" Height="32" Width="121" KeyDown="textBox1_KeyDown"/>
        <TextBox x:Name="textBox2" HorizontalAlignment="Left" Margin="213,167,0,0" TextWrapping="Wrap" VerticalAlignment="Top" Height="32" Width="121" KeyDown="textBox2_KeyDown"/>
        <TextBlock HorizontalAlignment="Left" Margin="60,226,0,0" TextWrapping="Wrap" Text="ObvNlat" VerticalAlignment="Top" Height="13" Width="127" FontSize="14" RenderTransformOrigin="0.5,0.5"/>
        <TextBox x:Name="textBox3" HorizontalAlignment="Left" Margin="213,207,0,0" TextWrapping="Wrap" VerticalAlignment="Top" Height="32" Width="121"/>
        <TextBox x:Name="textBox4" HorizontalAlignment="Left" Margin="213,244,0,0" TextWrapping="Wrap" VerticalAlignment="Top" RenderTransformOrigin="1.474,0.469" Height="32" Width="121"/>
        <TextBlock HorizontalAlignment="Left" Margin="60,263,0,0" TextWrapping="Wrap" Text="ObvElong" VerticalAlignment="Top" Height="13" Width="127" FontSize="14"/>
        <TextBox x:Name="textBox6" HorizontalAlignment="Left" Margin="213,323,0,0" TextWrapping="Wrap" VerticalAlignment="Top" Height="32" Width="121"/>
        <TextBlock HorizontalAlignment="Left" Margin="60,342,0,0" TextWrapping="Wrap" Text="CalDistance" VerticalAlignment="Top" Foreground="#FFF8F8F9" Height="13" Width="127" FontSize="14"/>
        <TextBox x:Name="textBox9" HorizontalAlignment="Left" Margin="566,130,0,0" TextWrapping="Wrap" VerticalAlignment="Top" Height="32" Width="111"/>
        <TextBox x:Name="textBox10" HorizontalAlignment="Left" Margin="566,189,0,0" TextWrapping="Wrap" VerticalAlignment="Top" Height="32" Width="111"/>
        <TextBlock HorizontalAlignment="Left" Margin="450,149,0,0" TextWrapping="Wrap" Text="Obv To Fir Ang" VerticalAlignment="Top" Height="13" Width="72" FontSize="14"/>
        <TextBlock HorizontalAlignment="Left" Margin="450,208,0,0" TextWrapping="Wrap" Text="Obv To Tar Ang" VerticalAlignment="Top" Height="13" Width="74" FontSize="14"/>
        <TextBox x:Name="textBox5" HorizontalAlignment="Left" Margin="566,498,0,0" TextWrapping="Wrap" VerticalAlignment="Top" Width="111" Height="32"/>
        <TextBlock HorizontalAlignment="Left" Margin="392,498,0,0" TextWrapping="Wrap" Text="Angle From Fir To Tar" VerticalAlignment="Top" FontSize="14" Height="17" Width="130"/>
        <TextBlock HorizontalAlignment="Left" Margin="319,596,0,0" TextWrapping="Wrap" Text="Fire To Target Distance" VerticalAlignment="Top" Foreground="Red" FontSize="22" Height="34" Width="231"/>
        <TextBox x:Name="textBox8" HorizontalAlignment="Left" Margin="566,598,0,0" TextWrapping="Wrap" VerticalAlignment="Top" Width="111" FontSize="16" Height="32"/>
        <TextBlock HorizontalAlignment="Left" Margin="60,10,0,0" TextWrapping="Wrap" Text="Observation 0.1" VerticalAlignment="Top" Width="291" Height="46" Foreground="#FFE6B7D3" FontSize="24"/>
        <TextBlock x:Name="ScenarioOutput_Latitude" HorizontalAlignment="Left" Margin="818,592,0,0" TextWrapping="Wrap" Text="No Lat Data" VerticalAlignment="Top" AllowDrop="False" FontSize="14" Height="17" Width="74"/>
        <TextBlock x:Name="ScenarioOutput_Longitude" HorizontalAlignment="Left" Margin="818,620,0,0" TextWrapping="Wrap" Text="No Long Data" VerticalAlignment="Top" FontSize="14" Height="17" Width="86"/>
        <Button x:Name="StartTrackingButton" Content="Star" HorizontalAlignment="Left" Margin="803,662,0,0" VerticalAlignment="Top" RenderTransformOrigin="-0.125,0.539" Click="StartTrackingButton_Click" Height="38" Width="60"/>
        <Button x:Name="StopTrackingButton" Content="Stop" HorizontalAlignment="Left" Margin="874,662,0,0" VerticalAlignment="Top" Click="StopTrackingButton_Click" Height="38" Width="65"/>
        <TextBlock x:Name="ScenarioOutput_Status" HorizontalAlignment="Left" Margin="818,563,0,0" TextWrapping="Wrap" Text="TextBlock" VerticalAlignment="Top" FontSize="14" Height="17" Width="57"/>
        <TextBlock HorizontalAlignment="Left" Margin="450,76,0,0" TextWrapping="Wrap" Text="Obser End" VerticalAlignment="Top" FontSize="22" Height="26" Width="101"/>
        <TextBlock HorizontalAlignment="Left" Margin="796,76,0,0" TextWrapping="Wrap" Text=" Fire End Double Check" VerticalAlignment="Top" FontSize="22" Height="26" Width="236"/>
        <TextBlock HorizontalAlignment="Left" Margin="796,508,0,0" TextWrapping="Wrap" Text="Observer Now Position" VerticalAlignment="Top" FontSize="22"/>
        <TextBlock HorizontalAlignment="Left" Margin="1061,508,0,0" TextWrapping="Wrap" Text="Fire Now Position" VerticalAlignment="Top" FontSize="22"/>
        <TextBox x:Name="textbox11" HorizontalAlignment="Left" Margin="890,186,0,0" TextWrapping="Wrap" Text="TextBox" VerticalAlignment="Top" Width="111"/>
        <Button x:Name="btnCalAzimuth" Content="Cal Azime" HorizontalAlignment="Left" Margin="890,124,0,0" VerticalAlignment="Top" RenderTransformOrigin="0.35,0.605" Width="111" Click="Button_Click"/>

    </Grid>
</Page>

//add 
using Windows.Devices.Geolocation;
using System.Threading.Tasks;
using Windows.UI.Core;


// 空白頁項目範本已記錄在 http://go.microsoft.com/fwlink/?LinkId=234238

namespace App002
{
          
    /// <summary>
    /// 可以在本身使用或巡覽至框架內的空白頁面。
    /// </summary>
    public sealed partial class MainPage : Page
    {

        public static MainPage Current;
        MainPage rootPage = MainPage.Current;
        private Geolocator _geolocator = null; 

        public MainPage()
        {
            this.InitializeComponent();
            //Geo
            Current = this;            
            _geolocator = new Geolocator();
        }

        // my goubal variable
        double fireNlat = -1;
        double fireElong = -1;
        double obvNlat = -1;
        double obvElong = -1;
        double d = 0;//觀察到火點距離  射擊  觀測間 距離
        //double td; // do my self test
        double R = 6378137;//km.meter
        //float compassdegree;

        /// <summary>
        /// 在此頁面即將顯示在框架中時叫用。
        /// </summary>
        /// <param name="e">描述如何到達此頁面的事件資料。Parameter
        /// 屬性通常用來設定頁面。</param>
        protected override void OnNavigatedTo(NavigationEventArgs e)
        {
            //StartTrackingButton.IsEnabled = true;
            //StopTrackingButton.IsEnabled = false;           
                
        }


        // Geo  
        #region  //  Geolocator
     

        public const string FEATURE_NAME = "Geolocator";
        

        /// <summary>
        ///
        /// </summary>
        /// <param name="sender"></param>
        /// <param name="e"></param>
        ///         
        protected override void OnNavigatingFrom(NavigatingCancelEventArgs e)
        {
            if (StopTrackingButton.IsEnabled)
            {
                _geolocator.PositionChanged -= new TypedEventHandler<Geolocator, PositionChangedEventArgs>(OnPositionChanged);
                _geolocator.StatusChanged -= new TypedEventHandler<Geolocator, StatusChangedEventArgs>(OnStatusChanged);
            }

            base.OnNavigatingFrom(e);
        }




        async private void OnPositionChanged(Geolocator sender, PositionChangedEventArgs e)
        {
            await Dispatcher.RunAsync(CoreDispatcherPriority.Normal, () =>
            {
                Geoposition pos = e.Position;

                //rootPage.NotifyUser("Updated", NotifyType.StatusMessage);

                ScenarioOutput_Latitude.Text = pos.Coordinate.Latitude.ToString();
                ScenarioOutput_Longitude.Text = pos.Coordinate.Longitude.ToString();
                //obvNlat = myConvert(double.Parse(pos.Coordinate.Latitude.ToString()));
                //obvElong = myConvert(double.Parse(pos.Coordinate.Longitude.ToString()));
                obvNlat = skConvert(double.Parse(pos.Coordinate.Latitude.ToString()));
                obvElong = skConvert(double.Parse(pos.Coordinate.Longitude.ToString()));
                textBox3.Text = pos.Coordinate.Latitude.ToString();
                textBox4.Text = pos.Coordinate.Longitude.ToString();
                //ScenarioOutput_Accuracy.Text = pos.Coordinate.Accuracy.ToString();
            });
        }
        
        async private void OnStatusChanged(Geolocator sender, StatusChangedEventArgs e)
        {
            await Dispatcher.RunAsync(CoreDispatcherPriority.Normal, () =>
            {
                switch (e.Status)
                {
                    case PositionStatus.Ready:
                        // Location platform is providing valid data.
                        ScenarioOutput_Status.Text = "Ready";
                        break;

                    case PositionStatus.Initializing:
                        // Location platform is acquiring a fix. It may or may not have data. Or the data may be less accurate.
                        ScenarioOutput_Status.Text = "Initializing";
                        break;

                    case PositionStatus.NoData:
                        // Location platform could not obtain location data.
                        ScenarioOutput_Status.Text = "No data";
                        break;

                    case PositionStatus.Disabled:
                        // The permission to access location data is denied by the user or other policies.
                        ScenarioOutput_Status.Text = "Disabled";

                        //Clear cached location data if any
                        ScenarioOutput_Latitude.Text = "No data";
                        ScenarioOutput_Longitude.Text = "No data";
                        //ScenarioOutput_Accuracy.Text = "No data";
                        break;

                    case PositionStatus.NotInitialized:
                        // The location platform is not initialized. This indicates that the application has not made a request for location data.
                        ScenarioOutput_Status.Text = "Not initialized";
                        break;

                    case PositionStatus.NotAvailable:
                        // The location platform is not available on this version of the OS.
                        ScenarioOutput_Status.Text = "Not available";
                        break;

                    default:
                        ScenarioOutput_Status.Text = "Unknown";
                        break;
                }
            });
        }
        


        public enum NotifyType
        {
            StatusMessage,
            ErrorMessage
        }

        private void StartTrackingButton_Click(object sender, RoutedEventArgs e)
        {
            _geolocator.PositionChanged += new TypedEventHandler<Geolocator, PositionChangedEventArgs>(OnPositionChanged);
            _geolocator.StatusChanged += new TypedEventHandler<Geolocator, StatusChangedEventArgs>(OnStatusChanged);

            StartTrackingButton.IsEnabled = false;
            StopTrackingButton.IsEnabled = true;
        }

        private void StopTrackingButton_Click(object sender, RoutedEventArgs e)
        {
            _geolocator.PositionChanged -= new TypedEventHandler<Geolocator, PositionChangedEventArgs>(OnPositionChanged);
            _geolocator.StatusChanged -= new TypedEventHandler<Geolocator, StatusChangedEventArgs>(OnStatusChanged);

            StartTrackingButton.IsEnabled = true;
            StopTrackingButton.IsEnabled = false;


        }


        #endregion
        // end GEO


        // compass
        #region  //  Compass

        #endregion
        // end compass

        private void Button_Click_1(object sender, RoutedEventArgs e)
        {


            #region //捉取兩位置經緯度                        
            if (textBox1.Text=="")
            {
                return;
            }        
            
            fireNlat = skConvert(double.Parse(textBox1.Text));
            if (textBox2.Text=="")
            {
                return;
            }       
            
            fireElong = skConvert(double.Parse(textBox2.Text));
            
            // obvNlat = skConvert(double.Parse(textBox3.Text));
            // obvElong = skConvert(double.Parse(textBox4.Text));

            d = Math.Acos(Math.Sin(fireNlat) * Math.Sin(obvNlat) + Math.Cos(fireNlat) * Math.Cos(obvNlat) * Math.Cos(Math.Abs(obvElong - fireElong))) * R;

            textBox6.Text = d.ToString(); // Fire to obv distance

            #endregion    
            //TEST station between 
            //建立誤差修正  台北火車站  textBox7
            
            #region //  自我測試 test only 適用範例
            /*
            //double taipeistationNlat = 25.047924;//fir
            //double taiperstationElong = 121.517081;

            // 台中火車站
            double taighungStNlat = 24.136845;//fir
            taighungStNlat = skConvert(taighungStNlat);
            double taichungStElong = 120.685009;
            taichungStElong = skConvert(taichungStElong);
            // 建立誤差修正  台中豐原車站
            double taichungFstationNlat = 24.254112;//obv
            taichungFstationNlat = skConvert(taichungFstationNlat);
            double taichungFstationElong = 120.722917;
            taichungFstationElong = skConvert(taichungFstationElong);
            ///  北中距離
            //double td = Math.Acos(Math.Sin(taipeistationNlat) * Math.Sin(taichungstationNlat) + Math.Cos(taipeistationNlat) * Math.Cos(taichungstationNlat) * Math.Cos(taichungstationElong- taiperstationElong)) * R;
            //textBox7.Text = td.ToString();
            // 中中距離

            td = Math.Acos(Math.Sin(taighungStNlat) * Math.Sin(taichungFstationNlat) + Math.Cos(taighungStNlat) * Math.Cos(taichungFstationNlat) * Math.Cos(taichungFstationElong - taichungStElong)) * R;
            textBox7.Text = td.ToString();
            */
            #endregion
            
            // computed azimuth
            double azimuth;                                                     
            azimuth = Math.Atan2(Math.Sin(fireElong - obvElong) * Math.Cos(fireNlat), Math.Cos(obvNlat) * Math.Sin(fireNlat) - Math.Sin(obvNlat) * Math.Cos(fireNlat) * Math.Cos(Math.Abs(fireElong - obvElong)));
            azimuth = azimuth * 180 / Math.PI;
            //azimuth = (azimuth + 180) % 360;
            textbox11.Text = azimuth.ToString();
            // transfer to mil system
            double milS;
            milS = azimuth * 6400 / 360;
            textBox10.Text = milS.ToString();


        }
        private void Button_Click(object sender, RoutedEventArgs e)
        {

        }

        #region  // skuld transulation
        private double skAlglecheck(double angle)
        {
            angle = angle % 360;
            return angle;
        }
        private double skConvert(double degree)
           // private double myConvert(double degree)//
        {
            return (Math.PI / 180) * degree;
        }
        #endregion


        #region    //  計算  火力射擊到目標距離
        private void btnFirToTar_Click(object sender, RoutedEventArgs e)
        {
            

            //double North = 0;//指北
            double thitaangle = 0;
            double ObvtoFireAng = -1;
            double ObvtoTarAng = -1;
            if (textBox9.Text == "")
            {
                return;
            }
            ObvtoFireAng = double.Parse(textBox9.Text);
            if (textBox10.Text == "")
            {
                return;
            }             
            ObvtoTarAng = double.Parse(textBox10.Text);


            thitaangle = Math.Abs(ObvtoTarAng - ObvtoFireAng);//  角火點經觀測到目標的夾角
            textBox5.Text = thitaangle.ToString();
            //接收COM port data


            //  計算火力發射點到目標距離                                  
            double firtotarD = 0;
            thitaangle = thitaangle % 90;
            firtotarD = d * Math.Tan(thitaangle * Math.PI / 180);// d td 來自 火點 與 觀測距離              
            textBox8.Text = firtotarD.ToString();


        }
        #endregion

        private void textBox1_KeyDown(object sender, KeyRoutedEventArgs e)
        {
            if (e.ToString() ==string.Empty|(int)e.Key < 48 | (int)e.Key > 57)
                e.Handled = true;
        }

        private void textBox2_KeyDown(object sender, KeyRoutedEventArgs e)
        {
            if (e.ToString() ==string.Empty|(int)e.Key < 48 | (int)e.Key > 57)
                e.Handled = true;
        }




    }
