<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CNECCC PE | Health Data</title>
    
    <script src="https://cdnjs.cloudflare.com/ajax/libs/xlsx/0.18.5/xlsx.full.min.js"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600&family=Montserrat:wght@600;700&display=swap" rel="stylesheet">
    
    <style>
        :root {
            --primary: #1E3A8A; 
            --primary-light: #3B82F6; 
            --success: #10B981; 
            --danger: #EF4444; 
            --bg-page: #F3F4F6; 
            --text-main: #1F2937;
            --text-muted: #6B7280;
            --border-color: #E5E7EB;
        }

        body { font-family: 'Inter', sans-serif; background-color: var(--bg-page); margin: 0; padding: 30px 15px; color: var(--text-main); }
        .container { max-width: 700px; margin: 0 auto; }

        .admin-panel {
            background: #ffffff; border-radius: 12px; padding: 20px 24px; margin-bottom: 24px;
            box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.05); border: 1px solid var(--border-color);
            border-left: 6px solid var(--primary-light);
        }
        .admin-header { display: flex; justify-content: space-between; align-items: center; flex-wrap: wrap; gap: 15px; margin-bottom: 15px;}
        .admin-panel h2 { font-family: 'Montserrat', sans-serif; margin: 0 0 4px 0; font-size: 18px; color: var(--primary); }
        .admin-panel p { margin: 0; color: var(--text-muted); font-size: 14px; font-weight: 500; }
        
        .db-upload {
            background: #EFF6FF; padding: 12px; border-radius: 8px; border: 1px dashed var(--primary-light);
            font-size: 13px; color: var(--primary); display: flex; align-items: center; gap: 10px;
        }
        
        .card { background: #FFFFFF; border-radius: 16px; box-shadow: 0 4px 15px rgba(0, 0, 0, 0.03); padding: 32px; margin-bottom: 20px; border: 1px solid rgba(0,0,0,0.05); }
        
        .header-card { background: linear-gradient(135deg, var(--primary) 0%, #312E81 100%); color: white; border: none; text-align: center; }
        h1 { font-family: 'Montserrat', sans-serif; font-size: 28px; margin-top: 0; margin-bottom: 8px; font-weight: 700; }
        .header-card p { color: #E0E7FF; font-size: 15px; line-height: 1.6; margin-bottom: 0; }

        .form-group { margin-bottom: 8px; }
        label { display: block; font-weight: 600; font-size: 16px; margin-bottom: 16px; color: var(--text-main); }
        .required { color: var(--danger); margin-left: 4px; }

        .id-card { background: linear-gradient(to right, #F0FDF4, #FFFFFF); border: 2px solid var(--success); padding: 24px; display: flex; align-items: center; transition: all 0.3s ease; }
        .id-card.empty { background: linear-gradient(to right, #F3F4F6, #FFFFFF); border: 2px dashed #D1D5DB; }
        .id-card .avatar { font-size: 45px; margin-right: 20px; }
        .id-card .status-label { color: var(--success); font-size: 12px; font-weight: 700; text-transform: uppercase; margin: 0 0 4px 0; letter-spacing: 1px;}
        .id-card.empty .status-label { color: var(--text-muted); }
        .id-card h3 { color: #064E3B; font-size: 22px; margin: 0; font-family: 'Montserrat', sans-serif; }
        .id-card.empty h3 { color: var(--text-muted); font-size: 18px; font-weight: 500; }

        .input-wrapper { position: relative; }
        .input-wrapper::after { content: attr(data-unit); position: absolute; right: 16px; top: 50%; transform: translateY(-50%); color: var(--text-muted); font-weight: 500; }
        
        input[type="number"] { width: 100%; padding: 14px 45px 14px 16px; border: 2px solid var(--border-color); border-radius: 10px; font-size: 16px; font-weight: 500; font-family: inherit; box-sizing: border-box; background-color: #F9FAFB; color: var(--primary); }
        input[type="number"]:invalid:not(:placeholder-shown) { border-color: var(--danger); background-color: #FEF2F2; }
        input[type="number"]:focus { outline: none; border-color: var(--primary-light); background-color: #fff; box-shadow: 0 0 0 4px rgba(59, 130, 246, 0.1); }

        .radio-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(90px, 1fr)); gap: 12px; }
        .radio-label { display: flex; align-items: center; cursor: pointer; padding: 12px; border: 2px solid var(--border-color); border-radius: 10px; font-weight: 500; transition: all 0.2s; }
        .radio-label:hover { border-color: var(--primary-light); background: #EFF6FF; }
        .radio-label input { margin-right: 10px; width: 18px; height: 18px; accent-color: var(--primary); }
        .radio-label:has(input:checked) { border-color: var(--primary); background-color: #EFF6FF; color: var(--primary); }

        .number-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(48px, 1fr)); gap: 10px; }
        .number-grid input[type="radio"] { display: none; }
        .number-box { display: flex; align-items: center; justify-content: center; height: 48px; background-color: #FFFFFF; border: 2px solid var(--border-color); border-radius: 12px; font-size: 16px; font-weight: 600; color: var(--text-muted); cursor: pointer; transition: all 0.15s ease-in-out; }
        .number-grid input[type="radio"]:hover:not(:checked) + .number-box { border-color: var(--primary-light); color: var(--primary-light); transform: translateY(-2px); }
        .number-grid input[type="radio"]:checked + .number-box { background-color: var(--primary); border-color: var(--primary); color: white; box-shadow: 0 4px 10px rgba(30, 58, 138, 0.3); transform: scale(1.05); }

        button { font-family: 'Inter', sans-serif; border: none; padding: 12px 24px; font-size: 14px; border-radius: 8px; cursor: pointer; font-weight: 600; transition: all 0.2s; }
        .btn-submit { background-color: var(--success); color: white; width: 100%; font-size: 16px; padding: 16px; border-radius: 12px; }
        .btn-submit:hover { background-color: #059669; }
        .btn-export { background-color: var(--primary); color: white; }
        .btn-export:hover { background-color: #1E40AF; }
        .btn-clear { background-color: transparent; color: var(--danger); border: 1px solid var(--border-color); }
        .btn-clear:hover { background-color: #FEF2F2; border-color: #F87171; }
        
        #recordCount { background: #D1FAE5; color: #065F46; padding: 2px 10px; border-radius: 12px; font-size: 14px; margin-left: 6px; }
        #dbStatus { font-weight: 700; color: var(--primary-light); }
        .footer-card { background: transparent; box-shadow: none; padding: 0; border: none; }
    </style>
</head>
<body>

<div class="container">
    <div class="admin-panel">
        <div class="admin-header">
            <div>
                <h2>📊 PE Data Dashboard</h2>
                <p>Database Status: <span id="dbStatus">🔄 Connecting to Server...</span></p>
                <p style="margin-top: 5px;">Records entered: <span id="recordCount">0</span></p>
            </div>
            
            <div style="display: flex; gap: 10px;">
                <button type="button" class="btn-clear" onclick="clearMeasurements()">🗑️ Clear Data</button>
                <button type="button" class="btn-export" onclick="exportToExcel()">📥 Export Full CSV List</button>
            </div>
        </div>
        
        <div class="db-upload" id="uploadSection" style="display: none;">
            <label for="excelUpload"><strong>Manual Override - Upload Student List:</strong></label>
            <input type="file" id="excelUpload" accept=".xlsx, .xls, .csv" onchange="manualUpload(event)">
        </div>
    </div>

    <form id="healthDataForm" onsubmit="saveData(event)">
        <div class="card header-card">
            <h1>🏃🏽‍♂️ CNECCC Physical Education</h1>
            <p>Body Measurement Data Entry. Height/ weight.</p>
        </div>

        <div class="card">
            <div class="form-group">
                <label>Academic Form <span class="required">*</span></label>
                <div class="radio-grid">
                    <label class="radio-label"><input type="radio" name="formGrade" value="1" onclick="lookupStudent()" required> F.1</label>
                    <label class="radio-label"><input type="radio" name="formGrade" value="2" onclick="lookupStudent()"> F.2</label>
                    <label class="radio-label"><input type="radio" name="formGrade" value="3" onclick="lookupStudent()"> F.3</label>
                    <label class="radio-label"><input type="radio" name="formGrade" value="4" onclick="lookupStudent()"> F.4</label>
                    <label class="radio-label"><input type="radio" name="formGrade" value="5" onclick="lookupStudent()"> F.5</label>
                    <label class="radio-label"><input type="radio" name="formGrade" value="6" onclick="lookupStudent()"> F.6</label>
                </div>
            </div>
        </div>

        <div class="card">
            <div class="form-group">
                <label>Class Section <span class="required">*</span></label>
                <div class="radio-grid">
                    <label class="radio-label"><input type="radio" name="studentClass" value="A" onclick="lookupStudent()" required> Class A</label>
                    <label class="radio-label"><input type="radio" name="studentClass" value="B" onclick="lookupStudent()"> Class B</label>
                    <label class="radio-label"><input type="radio" name="studentClass" value="C" onclick="lookupStudent()"> Class C</label>
                    <label class="radio-label"><input type="radio" name="studentClass" value="D" onclick="lookupStudent()"> Class D</label>
                </div>
            </div>
        </div>

        <div class="card">
            <div class="form-group">
                <label>Student Class Number <span class="required">*</span></label>
                <div class="number-grid" id="classNumberGrid">
                    </div>
            </div>
        </div>

        <div class="card id-card empty" id="studentProfileCard">
            <div class="avatar">👤</div>
            <div class="info">
                <p class="status-label" id="profileStatus">Awaiting Selection</p>
                <h3 id="displayName">Please select Form, Class, and Number</h3>
            </div>
        </div>

        <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px; margin-bottom: 20px;">
            <div class="card" style="margin-bottom: 0;">
                <div class="form-group">
                    <label for="height">Height (120 - 220 cm) <span class="required">*</span></label>
                    <div class="input-wrapper" data-unit="cm">
                        <input type="number" id="height" name="height" step="0.1" min="120" max="220" placeholder="e.g. 165.5" required>
                    </div>
                </div>
            </div>
            <div class="card" style="margin-bottom: 0;">
                <div class="form-group">
                    <label for="weight">Weight (20 - 150 kg) <span class="required">*</span></label>
                    <div class="input-wrapper" data-unit="kg">
                        <input type="number" id="weight" name="weight" step="0.1" min="20" max="150" placeholder="e.g. 55.2" required>
                    </div>
                </div>
            </div>
        </div>

        <div class="footer-card">
            <button type="submit" class="btn-submit">✅ Save Measurement & Next Student</button>
        </div>
    </form>
</div>

<script>
    let studentsDatabase = JSON.parse(localStorage.getItem('savedMeasurements')) || [];
    let schoolNamesDatabase = {};

    window.onload = function() {
        const grid = document.getElementById('classNumberGrid');
        for (let i = 1; i <= 40; i++) {
            grid.innerHTML += `<label><input type="radio" name="classNumber" value="${i}" onclick="lookupStudent()" required><div class="number-box">${i}</div></label>`;
        }
        updateRecordCount();

        // 🚀 AUTO-LOAD THE EMBEDDED EXCEL FILE
        fetch('student_list.xlsx')
            .then(response => {
                if (!response.ok) throw new Error("No bundled file found");
                return response.arrayBuffer();
            })
            .then(data => {
                const workbook = XLSX.read(new Uint8Array(data), {type: 'array'});
                parseWorkbook(workbook);
            })
            .catch(error => {
                console.log("No bundled student_list.xlsx detected.");
                document.getElementById('dbStatus').innerText = "❌ No Server Data Found";
                document.getElementById('uploadSection').style.display = "flex"; // Show manual upload as backup
            });
    };

    function parseWorkbook(workbook) {
        const firstSheetName = workbook.SheetNames[0];
        const worksheet = workbook.Sheets[firstSheetName];
        const rows = XLSX.utils.sheet_to_json(worksheet, {header: 1});
        
        const newDb = {};
        let clsIdx = -1, numIdx = -1, enIdx = -1, chIdx = -1;

        for (let i = 0; i < rows.length; i++) {
            const cols = rows[i];
            if (!cols || cols.length === 0) continue;

            if (clsIdx === -1) {
                for(let j=0; j<cols.length; j++) {
                    const val = String(cols[j] || '').trim().toUpperCase();
                    if (val === 'CLS_NAME' || /^[1-6][A-D]$/.test(val)) {
                        clsIdx = j; numIdx = j + 1; enIdx = j + 2; chIdx = j + 3; break;
                    }
                }
            }

            if (clsIdx !== -1 && cols.length > chIdx) {
                const clsName = String(cols[clsIdx] || '').trim().toUpperCase();
                const classNo = parseInt(String(cols[numIdx] || '').trim(), 10);
                const enName = String(cols[enIdx] || '').trim();
                const chName = String(cols[chIdx] || '').trim();
                
                if (/^[1-6][A-D]$/.test(clsName) && !isNaN(classNo)) {
                    const lookupKey = clsName + '-' + classNo;
                    newDb[lookupKey] = { en: enName, ch: chName };
                }
            }
        }

        if (Object.keys(newDb).length > 0) {
            schoolNamesDatabase = newDb;
            document.getElementById('dbStatus').innerText = "✅ Server Active (" + Object.keys(newDb).length + " students)";
            document.getElementById('uploadSection').style.display = "none";
            lookupStudent();
        }
    }

    // Manual fallback just in case
    function manualUpload(event) {
        const file = event.target.files[0];
        if (!file) return;
        const reader = new FileReader();
        reader.onload = function(e) {
            const data = new Uint8Array(e.target.result);
            const workbook = XLSX.read(data, {type: 'array'});
            parseWorkbook(workbook);
        };
        reader.readAsArrayBuffer(file);
    }

    function lookupStudent() {
        const formObj = document.querySelector('input[name="formGrade"]:checked');
        const classObj = document.querySelector('input[name="studentClass"]:checked');
        const numObj = document.querySelector('input[name="classNumber"]:checked');
        
        const card = document.getElementById('studentProfileCard');
        const nameDisplay = document.getElementById('displayName');
        const statusLabel = document.getElementById('profileStatus');

        if (formObj && classObj && numObj) {
            const lookupKey = formObj.value + classObj.value + "-" + numObj.value;
            const student = schoolNamesDatabase[lookupKey];

            if (student) {
                card.classList.remove('empty');
                statusLabel.innerText = `Currently Entering: ${formObj.value}${classObj.value} No. ${numObj.value}`;
                nameDisplay.innerText = `${student.en} (${student.ch})`;
                nameDisplay.style.color = "#064E3B"; 
            } else {
                card.classList.remove('empty');
                statusLabel.innerText = `⚠️ Missing Data: ${formObj.value}${classObj.value} No. ${numObj.value}`;
                nameDisplay.innerText = "No student found in database for this number";
                nameDisplay.style.color = "#EF4444"; 
            }
        } else {
            card.classList.add('empty');
            statusLabel.innerText = "Awaiting Selection";
            nameDisplay.innerText = "Please select Form, Class, and Number";
            nameDisplay.style.color = "#6B7280";
        }
    }

    function updateRecordCount() {
        document.getElementById('recordCount').innerText = studentsDatabase.length;
    }

    function saveData(event) {
        event.preventDefault(); 
        
        const formGrade = document.querySelector('input[name="formGrade"]:checked').value;
        const studentClass = document.querySelector('input[name="studentClass"]:checked').value;
        const classNumber = document.querySelector('input[name="classNumber"]:checked').value;
        const height = document.getElementById('height').value;
        const weight = document.getElementById('weight').value;

        const lookupKey = formGrade + studentClass + "-" + classNumber;
        const student = schoolNamesDatabase[lookupKey];
        const enName = student ? student.en : "";
        const chName = student ? student.ch : "";

        studentsDatabase = studentsDatabase.filter(r => r.lookupKey !== lookupKey);

        const newRecord = { 
            lookupKey,
            formGrade: "F." + formGrade, 
            studentClass, 
            classNumber, 
            enName, 
            chName, 
            height, 
            weight 
        };
        
        studentsDatabase.push(newRecord);
        localStorage.setItem('savedMeasurements', JSON.stringify(studentsDatabase));
        updateRecordCount();

        document.getElementById('height').value = '';
        document.getElementById('weight').value = '';
        const numberRadios = document.querySelectorAll('input[name="classNumber"]');
        numberRadios.forEach(radio => radio.checked = false);
        
        lookupStudent(); 
        
        const btn = document.querySelector('.btn-submit');
        const originalText = btn.innerHTML;
        btn.innerHTML = "💾 Saved Successfully!";
        btn.style.backgroundColor = "#059669";
        
        setTimeout(() => {
            btn.innerHTML = originalText;
            btn.style.backgroundColor = "";
            document.getElementById('height').focus(); 
        }, 800);
    }

    function exportToExcel() {
        if (Object.keys(schoolNamesDatabase).length === 0) {
            alert("⚠️ The student roster hasn't loaded properly. Can't export full list.");
            return;
        }

        const enteredDataMap = {};
        studentsDatabase.forEach(record => {
            enteredDataMap[record.lookupKey] = record;
        });

        let fullData = [];
        for (const [key, studentInfo] of Object.entries(schoolNamesDatabase)) {
            const splitIndex = key.indexOf('-');
            if (splitIndex === -1) continue;
            
            const clsName = key.substring(0, splitIndex); 
            const fNum = clsName.charAt(0); 
            const sClass = clsName.substring(1); 
            const cNum = parseInt(key.substring(splitIndex + 1), 10);

            const record = enteredDataMap[key];
            
            fullData.push({
                formNum: parseInt(fNum),
                formStr: "F." + fNum,
                classStr: sClass,
                classNum: cNum,
                enName: studentInfo.en,
                chName: studentInfo.ch,
                height: record ? record.height : "", 
                weight: record ? record.weight : ""  
            });
        }

        fullData.sort((a, b) => {
            if (a.formNum !== b.formNum) return a.formNum - b.formNum;
            if (a.classStr !== b.classStr) return a.classStr.localeCompare(b.classStr);
            return a.classNum - b.classNum;
        });

        let csvContent = "Form,Class,Class Number,English Name,Chinese Name,Height (cm),Weight (kg)\n";
        fullData.forEach(row => {
            csvContent += `${row.formStr},${row.classStr},${row.classNum},${row.enName},${row.chName},${row.height},${row.weight}\n`;
        });

        const BOM = "\uFEFF"; 
        const blob = new Blob([BOM + csvContent], { type: 'text/csv;charset=utf-8;' });
        const link = document.createElement("a");
        link.href = URL.createObjectURL(blob);
        link.download = "PE_Full_Class_List_Data.csv";
        link.click();
    }

    function clearMeasurements() {
        if (confirm("⚠️ This will clear the heights and weights you have entered. It will NOT delete the student names. Proceed?")) {
            studentsDatabase = [];
            localStorage.removeItem('savedMeasurements');
            updateRecordCount();
            alert("Measurements cleared. Ready for a new batch.");
        }
    }
</script>

</body>
</html>
