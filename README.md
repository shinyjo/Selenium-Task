# Selenium-Task
package sample;
import org.openqa.selenium.By; import org.openqa.selenium.WebDriver; import org.openqa.selenium.firefox.FirefoxDriver;
public class Demo {
public static void main(String[] args) {
    // TODO Auto-generated method stub

WebDriver driver=new FirefoxDriver();

driver.get("https://accounts.google.com/SignUp?service=mail&continue=https%3A%2F%2Fmail.google.com%2Fmail%2F%3Ftab%3Dwm&ltmpl=default");
driver.manage().window().maximize();
driver.findElement(By.id("FirstName")).sendKeys("A");
driver.findElement(By.id("lastname")).sendKeys("Shiny");
driver.findElement(By.id("GmailAddress")).sendKeys("Shinythea");
driver.findElement(By.id("Passwd")).sendKeys("July@2015");
driver.findElement(By.id("PasswdAgain")).sendKeys("July@2015");
driver.findElement(By.id("RecoveryPhoneNumber")).sendKeys("9944556739");
driver.findElement(By.id("RecoveryEmailAddress")).sendKeys("shinyjoji23@gmail.com");
driver.findElement(By.id("RecoveryEmailAddress")).sendKeys("shinyjoji23@gmail.com");
driver.findElement(By.id("SkipCaptcha")).click();
driver.findElement(By.id("submitbutton")).click();





}
}
