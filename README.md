package HomePage;

import org.openqa.selenium.WebDriver;
import org.openqa.selenium.chrome.ChromeDriver;

public class AmazonHomepage {
          public static void main(String[] args) {
 System.setProperty("webdriver.chrome.driver", "D:\\\\selenium_files\\\Chrome   driver\\\chromedriver.exe");
WebDriver driver = new ChromeDrive();
 driver.get("https://www.amazon.in/");
String expectedPageTitle = "Online Shopping site in India: Shop Online for Mobiles, Books, Watches, Shoes and More - Amazon.in";
String actualPageTitle = driver.getTitle();
 if (actualPageTitle.equals(expectedPageTitle)) {
 System.out.println("Amazon Homepage Title is verified Successfully .");
 } else {
 System.out.println("Amazon Homepage Title verification failed.");
System.out.println("Expected Page Title: " + expectedPageTitle);
System.out.println("Actual Page Title: " + actualPageTitle);
driver.quit();
	}
}
}
