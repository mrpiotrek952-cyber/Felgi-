<!DOCTYPE html>
<html lang="pl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Konfigurator Felg PRO</title>
    <style>
        body {
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
            background-color: #f0f2f5;
            color: #333;
            margin: 0;
            padding: 20px;
        }
        .container {
            max-width: 900px;
            margin: 0 auto;
            background: #fff;
            padding: 25px;
            border-radius: 12px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.05);
        }
        h2 {
            text-align: center;
            margin-top: 0;
            color: #2c3e50;
        }
        .database-section, .upload-section {
            display: flex;
            justify-content: space-between;
            gap: 20px;
            margin-bottom: 20px;
            background: #f8f9fa;
            padding: 15px;
            border-radius: 8px;
            border: 1px solid #e9ecef;
        }
        .control-box {
            flex: 1;
            display: flex;
            flex-direction: column;
            gap: 8px;
        }
        .control-box label {
            font-weight: 600;
            font-size: 14px;
        }
        select, input[type="file"] {
            padding: 8px;
            border-radius: 5px;
            border: 1px solid #ccc;
            font-family: inherit;
        }
        .divider {
            text-align: center;
            margin: -10px 0 10px 0;
            font-size: 12px;
            color: #888;
            text-transform: uppercase;
            letter-spacing: 2px;
        }
        .preview-container {
            position: relative;
            width: 100%;
            border: 2px dashed #ccc;
            border-radius: 8px;
            overflow: hidden;
            background-color: #fafafa;
            min-height: 300px;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        #carImage {
            width: 100%;
            height: auto;
            display: none; 
            pointer-events: none;
        }
        .rim {
            position: absolute;
            background-size: contain;
            background-repeat: no-repeat;
            background-position: center;
            display: none;
            z-index: 10;
        }
        /* Usuwamy domyślne transform, będziemy pozycjonować środkiem przez JS */
        #frontRim, #rearRim {
            transform: translate(-50%, -50%);
        }
        
        .controls-wrapper {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 30px;
            margin-top: 25px;
        }
        .control-panel {
            background: #fff;
            border: 1px solid #e1e4e8;
            padding: 20px;
            border-radius: 8px;
        }
        .control-panel h3 {
            margin-top: 0;
            font-size: 16px;
            border-bottom: 1px solid #eee;
            padding-bottom: 10px;
        }
        .slider-group {
            margin-bottom: 15px;
        }
        .slider-group label {
            display: flex;
            justify-content: space-between;
            font-size: 13px;
            margin-bottom: 5px;
            color: #555;
        }
        input[type="range"] {
            width: 100%;
            cursor: pointer;
        }
        .footer {
            text-align: center;
            margin-top: 30px;
            font-size: 12px;
            color: #888;
            font-weight: bold;
            letter-spacing: 1px;
        }
    </style>
</head>
<body>

<div class="container">
    <h2>Wirtualna Przymierzalnia Felg</h2>
    
    <!-- BAZA DANYCH -->
    <div class="database-section">
        <div class="control-box">
            <label for="carSelect">Wybierz samochód z bazy:</label>
            <select id="carSelect">
                <option value="">-- Wybierz auto --</option>
            </select>
        </div>
        <div class="control-box">
            <label for="rimSelect">Wybierz felgę z bazy:</label>
            <select id="rimSelect">
                <option value="">-- Wybierz felgę --</option>
            </select>
        </div>
    </div>

    <div class="divider">lub</div>

    <!-- RĘCZNY UPLOAD -->
    <div class="upload-section">
        <div class="control-box">
            <label for="carUpload">Wgraj własne zdjęcie auta (JPG/PNG)</label>
            <input type="file" id="carUpload" accept="image/*">
        </div>
        <div class="control-box">
            <label for="rimUpload">Wgraj własną felgę (tylko PNG bez tła)</label>
            <input type="file" id="rimUpload" accept="image/png">
        </div>
    </div>

    <div class="preview-container">
        <span id="placeholderText">Wybierz auto z bazy lub wgraj własne zdjęcie</span>
        <img id="carImage" src="" alt="Samochód">
        <div id="frontRim" class="rim"></div>
        <div id="rearRim" class="rim"></div>
    </div>

    <div class="controls-wrapper">
        <!-- Oś Przednia -->
        <div class="control-panel">
            <h3>Koło Przednie (Korekta)</h3>
            <div class="slider-group">
                <label>Rozmiar <span><span id="fSizeVal">100</span>%</span></label>
                <input type="range" id="fSize" min="20" max="300" value="100">
            </div>
            <div class="slider-group">
                <label>Pozycja X (Przód - Tył) <span><span id="fXVal">20</span>%</span></label>
                <input type="range" id="fX" min="0" max="100" value="20" step="0.5">
            </div>
            <div class="slider-group">
                <label>Pozycja Y (Góra - Dół) <span><span id="fYVal">50</span>%</span></label>
                <input type="range" id="fY" min="0" max="100" value="50" step="0.5">
            </div>
        </div>

        <!-- Oś Tylna -->
        <div class="control-panel">
            <h3>Koło Tylne (Korekta)</h3>
            <div class="slider-group">
                <label>Rozmiar <span><span id="rSizeVal">100</span>%</span></label>
                <input type="range" id="rSize" min="20" max="300" value="100">
            </div>
            <div class="slider-group">
                <label>Pozycja X (Przód - Tył) <span><span id="rXVal">75</span>%</span></label>
                <input type="range" id="rX" min="0" max="100" value="75" step="0.5">
            </div>
            <div class="slider-group">
                <label>Pozycja Y (Góra - Dół) <span><span id="rYVal">50</span>%</span></label>
                <input type="range" id="rY" min="0" max="100" value="50" step="0.5">
            </div>
        </div>
    </div>

    <div class="footer">
        powered by Greg K
    </div>
</div>

<script>
    // --- BAZA DANYCH (Zmień ścieżki do swoich plików!) ---
    
    // Dla każdego auta definiujemy gdzie domyślnie znajdują się osie (w procentach)
    const carsDB = [
        { id: "golf7", name: "Volkswagen Golf VII", src: "img/cars/golf7.jpg", fX: 18, fY: 62, fSize: 110, rX: 82, rY: 62, rSize: 110 },
        { id: "bmw_e90", name: "BMW Seria 3 (E90)", src: "img/cars/bmw_e90.jpg", fX: 20, fY: 65, fSize: 115, rX: 78, rY: 65, rSize: 115 },
        { id: "audi_a4", name: "Audi A4 B8", src: "img/cars/audi_a4.jpg", fX: 22, fY: 60, fSize: 105, rX: 79, rY: 60, rSize: 105 }
    ];

    const rimsDB = [
        { id: "bbs_rs", name: "BBS RS (Klasyka)", src: "img/rims/bbs_rs.png" },
        { id: "japan_racing", name: "Japan Racing JR11", src: "img/rims/jr11.png" },
        { id: "oz_superleggera", name: "OZ Superleggera", src: "img/rims/oz.png" }
    ];

    // --- REFERENCJE DOM ---
    const carSelect = document.getElementById('carSelect');
    const rimSelect = document.getElementById('rimSelect');
    const carUpload = document.getElementById('carUpload');
    const rimUpload = document.getElementById('rimUpload');
    
    const carImage = document.getElementById('carImage');
    const placeholderText = document.getElementById('placeholderText');
    const frontRim = document.getElementById('frontRim');
    const rearRim = document.getElementById('rearRim');

    const fSize = document.getElementById('fSize'), fX = document.getElementById('fX'), fY = document.getElementById('fY');
    const rSize = document.getElementById('rSize'), rX = document.getElementById('rX'), rY = document.getElementById('rY');

    // --- INICJALIZACJA BAZY ---
    function initDatabase() {
        carsDB.forEach(car => {
            let option = document.createElement('option');
            option.value = car.id;
            option.textContent = car.name;
            carSelect.appendChild(option);
        });

        rimsDB.forEach(rim => {
            let option = document.createElement('option');
            option.value = rim.id;
            option.textContent = rim.name;
            rimSelect.appendChild(option);
        });
    }

    // --- OBSŁUGA ZDARZEŃ ---

    // Wybór auta z bazy
    carSelect.addEventListener('change', function() {
        const selectedCar = carsDB.find(c => c.id === this.value);
        if (selectedCar) {
            loadCarImage(selectedCar.src);
            // Ustawienie domyślnych pozycji suwaków dla danego auta
            setSliders(selectedCar.fX, selectedCar.fY, selectedCar.fSize, selectedCar.rX, selectedCar.rY, selectedCar.rSize);
            carUpload.value = ""; // Reset ręcznego uploada
        }
    });

    // Wybór felgi z bazy
    rimSelect.addEventListener('change', function() {
        const selectedRim = rimsDB.find(r => r.id === this.value);
        if (selectedRim) {
            loadRimImage(selectedRim.src);
            rimUpload.value = ""; 
        }
    });

    // Ręczny upload auta
    carUpload.addEventListener('change', function(e) {
        if (e.target.files && e.target.files[0]) {
            const url = URL.createObjectURL(e.target.files[0]);
            loadCarImage(url);
            carSelect.value = ""; 
        }
    });

    // Ręczny upload felgi
    rimUpload.addEventListener('change', function(e) {
        if (e.target.files && e.target.files[0]) {
            const url = URL.createObjectURL(e.target.files[0]);
            loadRimImage(url);
            rimSelect.value = ""; 
        }
    });

    // --- FUNKCJE POMOCNICZE ---

    function loadCarImage(src) {
        carImage.src = src;
        carImage.style.display = 'block';
        placeholderText.style.display = 'none';
    }

    function loadRimImage(src) {
        frontRim.style.backgroundImage = `url('${src}')`;
        rearRim.style.backgroundImage = `url('${src}')`;
        frontRim.style.display = 'block';
        rearRim.style.display = 'block';
    }

    function setSliders(f_X, f_Y, f_Size, r_X, r_Y, r_Size) {
        fX.value = f_X; fY.value = f_Y; fSize.value = f_Size;
        rX.value = r_X; rY.value = r_Y; rSize.value = r_Size;
        updateWheels();
    }

    function updateWheels() {
        document.getElementById('fSizeVal').innerText = fSize.value;
        document.getElementById('fXVal').innerText = fX.value;
        document.getElementById('fYVal').innerText = fY.value;
        document.getElementById('rSizeVal').innerText = rSize.value;
        document.getElementById('rXVal').innerText = rX.value;
        document.getElementById('rYVal').innerText = rY.value;

        frontRim.style.width = `${fSize.value}px`;
        frontRim.style.height = `${fSize.value}px`;
        frontRim.style.left = `${fX.value}%`;
        frontRim.style.top = `${fY.value}%`;

        rearRim.style.width = `${rSize.value}px`;
        rearRim.style.height = `${rSize.value}px`;
        rearRim.style.left = `${rX.value}%`;
        rearRim.style.top = `${rY.value}%`;
    }

    const sliders = [fSize, fX, fY, rSize, rX, rY];
    sliders.forEach(slider => {
        slider.addEventListener('input', updateWheels);
    });

    // Odpal inicjalizację po załadowaniu
    initDatabase();
</script>

</body>
</html>
