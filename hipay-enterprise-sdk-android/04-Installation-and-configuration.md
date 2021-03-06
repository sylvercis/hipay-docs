# Installation

Before starting the installation, please read all instructions and make sure you've gone through the [Prerequisites and recommendations](#prerequisites-and-recommendations) section.

It's recommended to use *Gradle* to install the HiPay Enterprise SDK for Android.

## Using Gradle (recommended)

Add this line to your project's `build.gradle`:

	dependencies { 
		compile 'com.hipay.fullservice:hipayfullservice:1+'
	}

Then synchronize the project with Gradle files. This will install the core wrapper components as well as the built-in payment screen and other utility components.

# Configuration

You need to provide the SDK with a few parameters, such as the credentials and targeted environment.

## Credentials

Get a valid HiPay Enterprise API username and password. If you don't have any, please refer to the [Prerequisites and recommendations](#prerequisites-and-recommendations) section.

## Setting up the configuration

The following code allows you to configure the SDK. We recommend putting it in your *App Launcher Activity*'s `onCreate()` method implementation.

```Java
public class DemoActivity extends AppCompatActivity {
     ...

     protected void onCreate(Bundle savedInstanceState) {
         super.onCreate(savedInstanceState);
         
         ClientConfig.getInstance().setConfig(
         
                ClientConfig.Environment.Stage,
                "YOUR API USERNAME",
                "YOUR API PASSWORD"
        );
     }

     //optional features

     ClientConfig.getInstance().setPaymentCardStorageEnabled(true);

     ClientConfig.getInstance().setPaymentCardScanEnabled(true);

     ClientConfig.getInstance().setPaymentCardNfcScanEnabled(true);
}

```

Do not forget to **replace the username and password arguments with your API username and password**.

The Payment card storage option is also called "One-click payment".
You can find more information in the [Card storage feature](#usage-making-payments-core-wrapper-advanced-integration-card-storage-feature) page. 

The **camera scan** and **NFC scan** options help create a more fluid mobile payment process.    

 
Once your app goes live, you need to set the environment to `Environment.Production`.
