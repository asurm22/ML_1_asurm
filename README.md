# ML_1_asurm
კონკურსის მიმოხილვა

ეს პროექტი მიზნად ისახავს Kaggle-ის "House Prices: Advanced Regression Techniques" კონკურსში მონაწილეობას. ყველა ანალიზი და მოდელირება განხორციელებულია ერთ ფაილში assignment1_1.ipynb.

მიდგომა

პროექტი მოიცავს შემდეგ ეტაპებს:

მონაცემთა წინასწარი დამუშავება:
  NaN მნიშვნელობების დამუშავება
  კატეგორიული ცვლადების ტრანსფორმაცია
  ახალი ფიჩერების შექმნა
მოდელირება:
  (Linear Regression)
  (Random Forest)
  
ფაილის აღწერა

assignment1_1.ipynb - Jupyter Notebook, რომელიც შეიცავს:

მონაცემთა ჩატვირთვა და წინასწარი დამუშავება:
  HousePricePreprocessor კლასის გამოყენებით
  მნიშვნელოვანი NaN მნიშვნელობების დამუშავება
  ორდინალური და ნომინალური ცვლადების კოდირება
Feature Engineering:
  TotalSF (საერთო ფართობი)
  TotalPorchSF (აივნების საერთო ფართობი)
  HouseAge (სახლის ასაკი)
  TotalBathrooms (საერთო აბაზანების რაოდენობა)
მოდელირება და შეფასება:
  ხაზოვანი რეგრესია (Linear Regression)
  შემთხვევითი ტყე (Random Forest)
MLflow ინტეგრაცია:
  ექსპერიმენტების ჩაწერა
  მეტრიკების ლოგირება
  ექსპერიმენტების შედეგებზე დაკვირვება
  მათ მიხედვით ფიჩერების დააფდეითება
  საუკეთესო მოდელის შერჩევა

best rmse for linear: 0.16
best rmse for RFG: 0.14

საბოლოო მოდელი არჩეული იქნა Random Forest შემდეგი პარამეტრებით, რადგან ყველაზე დაბალი rmse ქონდა:

n_estimators=300,
max_depth=15,
min_samples_leaf=3,
random_state=42,
n_jobs=-1

საბოლოო კოდში ფიჩერებზე დაკვირვება და სხვადასხვა საბოლოოდ არა საჭირო კოდის
ნაწილები ამოვაკელი და დავტოვე მხოლოდ საბოლოო მოდელის შესადგენად საჭირო კოდი.

MLFlow experiments:
[Linear Regression](https://dagshub.com/asurm22/ML_1_asurm.mlflow/#/experiments/2?viewStateShareKey=3894e7dac091113a949e1a0b144bdfbf23f857b1cfb2b6251e919052fe25b155&compareRunsMode=TABLE)
[Random Forest](https://dagshub.com/asurm22/ML_1_asurm.mlflow/#/experiments/3?viewStateShareKey=3894e7dac091113a949e1a0b144bdfbf23f857b1cfb2b6251e919052fe25b155&compareRunsMode=TABLE)
