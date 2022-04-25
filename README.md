# SeleniumWebDriverSetUp
SeleniumWebDriverSetUp
// How to set up Selenium Web Driver with Visuoal Studio, 
// Package Manage r and instal Package Selenium.WebDriver  and Selenium WebDriver.chromeDriver (for diff browser different WebDriver Package)

Example: 

using OpenQA.Selenium;
using OpenQA.Selenium.Chrome;  // different for diff Browsers !!!!
using System;


class SeleniumExample
{
    static void Main()
    {
        IWebDriver driver = new ChromeDriver();  //create new instance of the driver
        driver.Navigate().GoToUrl("https://softuni.bg");  // deiver navigate to this url and open it
        
        Console.WriteLine(driver.Title);   //driver print the title of the opened Page
        driver.Quit(); //driver quit the resources -> close the instance of the Chrome !
    }
}

