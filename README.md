# MLOps Project: Property Price Forecast in Paris

![Captura de tela 2024-07-22 182910](https://github.com/user-attachments/assets/82243659-6852-4618-a66f-6d66b3f7c068)

**Deployment URL**: https://vercel-app-mlops-zoomcamp-project-paris-price-house.vercel.app.

----------------------------------------

### Project Overview
This project aims to predict house prices in the urban environment of Paris using a variety of features. The primary goal is to provide accurate property price estimations through machine learning models. This information will assist potential buyers, real estate agents, and developers in making well-informed decisions.

-------------------

![Captura de tela 2024-07-22 170053](https://github.com/user-attachments/assets/836c3ef3-d0c9-4afb-9258-79aa01db9f79)

### Dataset Description
The dataset used in this project consists of synthetic data on house prices in Paris. It includes numeric attributes representing various features of the properties. This dataset is particularly valuable for educational purposes, practice, and gaining knowledge in machine learning and data analysis.

The dataset can be found on Kaggle: [Paris Housing Price Prediction](https://www.kaggle.com/datasets/mssmartypants/paris-housing-price-prediction).

#### Context and Content do Dataset
This dataset is created from synthetic data representing house prices in the urban environment of Paris. It is ideal for educational purposes, practice, and gaining essential knowledge in machine learning and data analysis.

Next, the goal is to create a classification dataset from the existing data by adding a new column for the class attribute.

The dataset contains more than just rows and columns, it includes detailed house attributes listed as column names.

#### Description das colunas do Dataset
All attributes are numeric variables and are listed below:

- `squareMeters`: Total area of the house in square meters.
- `numberOfRooms`: Total number of rooms in the house.
- `hasYard`: Indicates whether the house has a yard (1 for yes, 0 for no).
- `hasPool`: Indicates whether the house has a pool (1 for yes, 0 for no).
- `floors`: Number of floors in the house.
- `cityCode`: Zip code of the house's location.
- `cityPartRange`: A range value indicating the exclusivity of the neighborhood; higher values denote more exclusive areas.
- `numPrevOwners`: Number of previous owners the house has had.
- `made`: Year the house was built.
- `isNewBuilt`: Indicates whether the house is newly built (1 for yes, 0 for no).
- `hasStormProtector`: Indicates whether the house has storm protection features (1 for yes, 0 for no).
- `basement`: Area of the basement in square meters.
- `attic`: Area of the attic in square meters.
- `garage`: Size of the garage in square meters.
- `hasStorageRoom`: Indicates whether the house has a storage room (1 for yes, 0 for no).
- `hasGuestRoom`: Number of guest rooms in the house.
- `price`: Predicted price value of the house.

- Dataset Size: ParisHousing.csv (633.42 kB)

- Tags: Real Estate; Hotels and Accommodations; Regression; Cities and Urban Areas; Housing; Linear Regression

- Dataset available at Kaggle: [Paris Housing Price Prediction](https://www.kaggle.com/datasets/mssmartypants/paris-housing-price-prediction)

-----------------------------------------------------

### Tech Stack

<div style="display: inline_block"><br>
  <img align="center" src="https://camo.githubusercontent.com/3d768e26ac10ba994a60ed19acd487895cc43a9cdd43e9305c2408b93136234d/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f6769742d2532334630353033332e7376673f7374796c653d666f722d7468652d6261646765266c6f676f3d676974266c6f676f436f6c6f723d7768697465">
  <img align="center" src="https://camo.githubusercontent.com/998382ebc9a32162128b00b597ea488192df024fd015e5edec001fe29fcb93a6/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f56697375616c25323053747564696f253230436f64652d3030373864372e7376673f7374796c653d666f722d7468652d6261646765266c6f676f3d76697375616c2d73747564696f2d636f6465266c6f676f436f6c6f723d7768697465">
    <img align="center" src="https://camo.githubusercontent.com/d0acc51aec2d81ad604d51506e176736b43c20a4328500849ac49a956b12b820/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4b6167676c652d3230424546463f7374796c653d666f722d7468652d6261646765266c6f676f3d4b6167676c65266c6f676f436f6c6f723d7768697465">
    <img align="center" src="https://camo.githubusercontent.com/0562f16a4ae7e35dae6087bf8b7805fb7e664a9e7e20ae6d163d94e56b94f32d/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f707974686f6e2d3336373041303f7374796c653d666f722d7468652d6261646765266c6f676f3d707974686f6e266c6f676f436f6c6f723d666664643534">
    <img align="center" src="https://camo.githubusercontent.com/ca8ee16f3ff90cf3349be99b021b0b2a366cd71499ef20bcdc2b43dbc2668483/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f416e61636f6e64612d2532333434413833332e7376673f7374796c653d666f722d7468652d6261646765266c6f676f3d616e61636f6e6461266c6f676f436f6c6f723d7768697465">
    <img align="center" src="https://camo.githubusercontent.com/c044ae9d0419850e7f2385c22ea5de56e101e6a616789bd35d2d8fa137a63642/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f6a7570797465722d2532334641304630302e7376673f7374796c653d666f722d7468652d6261646765266c6f676f3d6a757079746572266c6f676f436f6c6f723d7768697465">
      <img align="center" src="https://camo.githubusercontent.com/05cab52d05663cecbe47a23ca71075ba81b9080dd50561d0f76eb46e902cfef8/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f70616e6461732d2532333135303435382e7376673f7374796c653d666f722d7468652d6261646765266c6f676f3d70616e646173266c6f676f436f6c6f723d7768697465">
      <img align="center" src="https://camo.githubusercontent.com/edd8c9123ff9093143508af0b218cffc132f16a014be2d2147894458c351dc23/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4d6174706c6f746c69622d2532336439656164332e7376673f7374796c653d666f722d7468652d6261646765266c6f676f3d4d6174706c6f746c6962266c6f676f436f6c6f723d626c61636b">
      <img align="center" src="https://camo.githubusercontent.com/6854ba9612c2cb025e7c65445787d93f6436d4691303601506e0bc28be2ae9b8/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f506f737467726553514c2d3331363139323f7374796c653d666f722d7468652d6261646765266c6f676f3d706f737467726573716c266c6f676f436f6c6f723d7768697465">
      <img align="center" src="https://camo.githubusercontent.com/d7eb681a1d19819ff9caeee4e3b0b1748da0b97af47e2084ca3d5e8302aec8a9/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f7363696b69742d2d6c6561726e2d2532334637393331452e7376673f7374796c653d666f722d7468652d6261646765266c6f676f3d7363696b69742d6c6561726e266c6f676f436f6c6f723d7768697465">
      <img align="center" src="https://camo.githubusercontent.com/40b50389027e826f74eb106c67530673ffc46486250581ca5845fc7284f7c717/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4d4c666c6f772d3031393445322e7376673f7374796c653d666f722d7468652d6261646765266c6f676f3d4d4c666c6f77266c6f676f436f6c6f723d7768697465">
      <img align="center" src="https://camo.githubusercontent.com/9ed458fea6ba5324c019bbc32f837fbceaca74f3862454a77d7e94150b97fc48/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f666c61736b2d2532333030302e7376673f7374796c653d666f722d7468652d6261646765266c6f676f3d666c61736b266c6f676f436f6c6f723d7768697465">
      <img align="center" src="https://camo.githubusercontent.com/8396abd667a0eca7d28cdb29ec63b6bf29a7854c7c3d467e6ece648c7e9b81e1/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f646f636b65722d2532333064623765642e7376673f7374796c653d666f722d7468652d6261646765266c6f676f3d646f636b6572266c6f676f436f6c6f723d7768697465">
      <img align="center" src="https://camo.githubusercontent.com/a00920b123df05b3df5e368e509f18bacd65bc5909698fb42be5f35063550f47/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f747970657363726970742d2532333030374143432e7376673f7374796c653d666f722d7468652d6261646765266c6f676f3d74797065736372697074266c6f676f436f6c6f723d7768697465">
      <img align="center" src="https://camo.githubusercontent.com/65f3aaa6432363f0979f3e35bc4783d5b39753d50d200e0c149fc5c78e1eeb49/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4e6578742e6a732d626c75653f7374796c653d666f722d7468652d6261646765266c6f676f3d4e6578742e6a73266c6f676f436f6c6f723d7768697465253232">
        <img align="center" src="https://camo.githubusercontent.com/bfe42a01bfb74a48dabc254065e874f313ca2aedd9bde944cb8bb4f9cef69dd4/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f6e6f64652e6a732d3033363834663f7374796c653d666f722d7468652d6261646765266c6f676f3d6e6f64652e6a73266c6f676f436f6c6f723d7768697465"> 
      <img align="center" src="https://camo.githubusercontent.com/509859c3a417eb3ea794450d88303bdaced996cba60811e552e5a89bf89ff584/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f67726166616e612d2532334634363830302e7376673f7374796c653d666f722d7468652d6261646765266c6f676f3d67726166616e61266c6f676f436f6c6f723d7768697465">
        <img align="center" src="https://camo.githubusercontent.com/b9ff564d8c311812747f1aacea54cf703d850756f9179f9eff6899da20a701a2/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f76657263656c2d2532333030303030302e7376673f7374796c653d666f722d7468652d6261646765266c6f676f3d76657263656c266c6f676f436f6c6f723d7768697465">
      </div>

------------------------------------------------
### Paris Price House App

This is a Next.js and Python based ML application for house price prediction in Paris, France.

**Getting Started**
---------------

### Prerequisites

* Node.js installed on your machine
* Python installed on your machine

### Installation

1. Create a new Next.js app using the latest version of `create-next-app`:
```
npx create-next-app@latest paris-price-house
```
2. Change into the newly created app directory:
```
cd paris-price-house
```
3. Install Axios, a popular HTTP client library:
```
npm install axios
```

### Running the App

1. Run the Python script that fetches data from an external API:
```
python app.py
```
2. Start the Next.js development server:
```
npx next
```
This will start the development server and make the app available at `http://localhost:3000`.

--------------------------------------------------

### Deployment vercel-app-mlops-zoomcamp-project-paris-price-house.vercel.app

The project is deployed on Vercel, making it easily accessible for users. The deployment ensures that users can input property details through the frontend and get real-time price predictions.

### How to Use app vercel "Property Price Forecast in Paris"
- 1. Fill in all fields with property information: Enter information about the property in the input fields provided in the interface. Only positive numbers are allowed.
- 2. For fields where there is no information to be entered, they must be filled in with 0, indicating the absence.
- 3. If any field is not filled in, clicking the `"Estimate Price"` button will return the alert `"Please fill in all fields to get a forecast!"`
- 4. After filling in all the fields, click on the `“Estimate Price”` button to obtain the predicted price of the property.
- 5. The predicted price will be displayed on the screen, providing an estimate based on the input data. Example: `"Forecasted Price: €557642.1"`.
- 6. Click on the `"Clear Fields"` button so that all fields are reset.
 
--------------------------------------------------






