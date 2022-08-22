# TestVigrant
Class Screenshot
{ 
@BeforeClass
Public void openBrowser()
{
System.setProperty("webdriver.chrome.driver","./Drivers/Software/chromedriver.exe");
WebDriver driver=new ChromeDriver();
}
@Before Method()
{
driver.get("https://www.wikipedia.org");
driver.findElement(By.xpath("//input[@id='searchInput']"));
}
@Test
Public void take screenshot()
{
