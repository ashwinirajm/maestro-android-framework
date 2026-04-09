# maestro-android-framework

This repository contains an Android test automation framework built with Maestro for testing the Swag Labs Mobile App. The framework uses flows, config, and test data to maintain reusable, scalable, and readable test automation.

## SetUp
1. Clone the repo:
```
git clone https://github.com/ashwinirajm/maestro-android-framework.git
cd maestro-android-framework
```
2. Install Maestro
```
curl -Ls https://get.maestro.mobile.dev | bash
```
3. Set up android emulator
4. Run test
```
maestro test flows/e2e_flow.yaml
```

## Project Structure

```
maestro-android-framework/
├── flows/                     
│   ├── login.yaml
│   ├── logout.yaml
│   ├── add_to_cart.yaml
│   ├── cart_verification.yaml
│   ├── checkout.yaml
│   └── e2e_flow.yaml          
│
├── config/                    
│   ├── app.yaml               
│   └── devices.yaml           
│
├── test-data/                  
    ├── login_credentials.yaml
    └── products.yaml             
```


## Key Highlights

- **End-to-End Android Testing:** Covers login, logout, and purchase flows.  
- **Data-Driven:** Test data separated into YAML (`login_credentials`, `product_details`).  
- **Reusable Flows:** Individual YAML flows for login, logout, add-to-cart, checkout, and cart verification.  
- **Dynamic Locators & Logging:** Captures product description, price, and other dynamic elements.  
- **Automation Ready:** Supports Maestro automation for Android (React Native apps).  
- **Device-Specific Testing:** Can specify different emulators/devices in the config.  
- **Clear & Modular Structure:** `config`, `flows`, `test-data` directories for organized maintenance.  





