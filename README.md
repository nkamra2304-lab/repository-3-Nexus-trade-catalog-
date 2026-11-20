# repository-3-Nexus-trade-catalog-
(Device manufacturer database, models, and base pricing) 
const catalog = {
    'Apple': ['iPhone 15 Pro Max', 'iPhone 15 Pro', 'iPhone 15 Plus', 'iPhone 15', 'iPhone 14 Pro Max', 'iPhone 14 Pro', 'iPhone 13', 'iPhone 12', 'iPhone 11', 'iPhone SE (3rd Gen)'],
    'Samsung': ['Galaxy S24 Ultra', 'Galaxy S24+', 'Galaxy S24', 'Galaxy S23 Ultra', 'Galaxy S23+', 'Galaxy Z Fold5', 'Galaxy Z Flip5', 'Galaxy A54 5G', 'Galaxy A34 5G', 'Galaxy S21 FE'],
    'Realme': ['Realme GT 5 Pro', 'Realme GT 3', 'Realme 11 Pro+', 'Realme 11 Pro', 'Realme 10 Pro+', 'Realme Narzo 60 Pro', 'Realme GT Neo 3', 'Realme 9 Pro+', 'Realme C55', 'Realme 9i'],
    'Redmi': ['Redmi Note 13 Pro+', 'Redmi Note 13 Pro', 'Redmi Note 13', 'Redmi K60 Pro', 'Redmi Note 12 Pro+', 'Redmi Note 12', 'Redmi 13C', 'Redmi A2+', 'Redmi Note 11 Pro', 'Redmi 10 Prime'],
    'Google': ['Pixel 8 Pro', 'Pixel 8', 'Pixel 7a', 'Pixel 7 Pro', 'Pixel 7', 'Pixel 6a', 'Pixel 6 Pro', 'Pixel 6', 'Pixel 5', 'Pixel 4a'],
    'Oppo': ['Oppo Find X7 Ultra', 'Oppo Find N3', 'Oppo Reno 11 Pro', 'Oppo Reno 10 Pro+', 'Oppo Find X5 Pro', 'Oppo Reno 8', 'Oppo A78', 'Oppo A58', 'Oppo F23 Pro', 'Oppo Reno 7'],
    'Motorola': ['Moto Edge 50 Pro', 'Moto Razr 40 Ultra', 'Moto Edge 40', 'Moto G84 5G', 'Moto G54 5G', 'Moto Edge 30 Ultra', 'Moto G73', 'Moto One 5G', 'Moto G62', 'Moto E13'],
    'Vivo': ['Vivo X100 Pro', 'Vivo X90 Pro', 'Vivo V30 Pro', 'Vivo V29', 'Vivo X80 Pro', 'Vivo T2 Pro', 'Vivo Y200', 'Vivo V27', 'Vivo Y100', 'Vivo Y35'],
    'Poco': ['Poco F6 Pro', 'Poco X6 Pro', 'Poco X6', 'Poco F5', 'Poco X5 Pro', 'Poco M6 Pro', 'Poco C65', 'Poco F4 GT', 'Poco X4 Pro', 'Poco M5'],
    'OnePlus': ['OnePlus 12', 'OnePlus 12R', 'OnePlus Open', 'OnePlus 11', 'OnePlus 11R', 'OnePlus 10 Pro', 'OnePlus 10T', 'OnePlus Nord 3', 'OnePlus Nord CE 3', 'OnePlus 9 Pro'],
    'Nothing': ['Nothing Phone (2)', 'Nothing Phone (1)', 'Nothing Phone (2a)', 'Nothing Ear (2)', 'Nothing Ear (open)', 'Nothing Phone (2) Special', 'Nothing Phone (1) Alpha', 'Nothing Concept 1', 'Nothing OS Edition', 'Nothing Watch Pro']
};

const prices = {
    'iPhone 15 Pro Max': 890, 'iPhone 15 Pro': 720, 'iPhone 15 Plus': 610, 'iPhone 15': 550, 'iPhone 14 Pro Max': 680, 'iPhone 14 Pro': 540, 'iPhone 13': 370, 'iPhone 12': 280, 'iPhone 11': 190, 'iPhone SE (3rd Gen)': 160,
    'Galaxy S24 Ultra': 810, 'Galaxy S24+': 650, 'Galaxy S24': 560, 'Galaxy S23 Ultra': 590, 'Galaxy S23+': 490, 'Galaxy Z Fold5': 720, 'Galaxy Z Flip5': 430, 'Galaxy A54 5G': 210, 'Galaxy A34 5G': 170, 'Galaxy S21 FE': 220,
    'Realme GT 5 Pro': 400, 'Realme GT 3': 320, 'Realme 11 Pro+': 250, 'Realme 11 Pro': 210, 'Realme 10 Pro+': 180, 'Realme Narzo 60 Pro': 170, 'Realme GT Neo 3': 190, 'Realme 9 Pro+': 140, 'Realme C55': 90, 'Realme 9i': 70,
    'Redmi Note 13 Pro+': 260, 'Redmi Note 13 Pro': 210, 'Redmi Note 13': 150, 'Redmi K60 Pro': 310, 'Redmi Note 12 Pro+': 180, 'Redmi Note 12': 120, 'Redmi 13C': 80, 'Redmi A2+': 50, 'Redmi Note 11 Pro': 110, 'Redmi 10 Prime': 60,
    'Pixel 8 Pro': 520, 'Pixel 8': 400, 'Pixel 7a': 230, 'Pixel 7 Pro': 350, 'Pixel 7': 270, 'Pixel 6a': 180, 'Pixel 6 Pro': 220, 'Pixel 6': 150, 'Pixel 5': 110, 'Pixel 4a': 70,
    'Oppo Find X7 Ultra': 600, 'Oppo Find N3': 650, 'Oppo Reno 11 Pro': 280, 'Oppo Reno 10 Pro+': 300, 'Oppo Find X5 Pro': 340, 'Oppo Reno 8': 170, 'Oppo A78': 130, 'Oppo A58': 100, 'Oppo F23 Pro': 140, 'Oppo Reno 7': 120,
    'Moto Edge 50 Pro': 350, 'Moto Razr 40 Ultra': 480, 'Moto Edge 40': 270, 'Moto G84 5G': 160, 'Moto G54 5G': 120, 'Moto Edge 30 Ultra': 310, 'Moto G73': 130, 'Moto One 5G': 90, 'Moto G62': 80, 'Moto E13': 45,
    'Vivo X100 Pro': 580, 'Vivo X90 Pro': 450, 'Vivo V30 Pro': 310, 'Vivo V29': 240, 'Vivo X80 Pro': 330, 'Vivo T2 Pro': 150, 'Vivo Y200': 130, 'Vivo V27': 200, 'Vivo Y100': 110, 'Vivo Y35': 80,
    'Poco F6 Pro': 380, 'Poco X6 Pro': 290, 'Poco X6': 210, 'Poco F5': 260, 'Poco X5 Pro': 190, 'Poco M6 Pro': 130, 'Poco C65': 70, 'Poco F4 GT': 220, 'Poco X4 Pro': 140, 'Poco M5': 80,
    'OnePlus 12': 550, 'OnePlus 12R': 410, 'OnePlus Open': 700, 'OnePlus 11': 430, 'OnePlus 11R': 320, 'OnePlus 10 Pro': 280, 'OnePlus 10T': 250, 'OnePlus Nord 3': 210, 'OnePlus Nord CE 3': 160, 'OnePlus 9 Pro': 200,
    'Nothing Phone (2)': 350, 'Nothing Phone (1)': 200, 'Nothing Phone (2a)': 230, 'Nothing Ear (2)': 60, 'Nothing Ear (open)': 70, 'Nothing Phone (2) Special': 380, 'Nothing Phone (1) Alpha': 190, 'Nothing Concept 1': 150, 'Nothing OS Edition': 120, 'Nothing Watch Pro': 50
};
