here<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <title>فرم ثبت اطلاعات کاربر</title>
    <style>
        body {
            font-family: "Vazir", sans-serif;
            background-color: #f9f9f9;
            padding: 20px;
            text-align: center;
        }

        form {
            background-color: #fff;
            padding: 20px;
            border-radius: 12px;
            box-shadow: 0 0 8px rgba(0,0,0,0.1);
            width: 60%;
            margin: auto;
        }

        label {
            display: inline-block;
            width: 150px;
            text-align: right;
            margin-bottom: 10px;
        }

        input, select {
            padding: 5px;
            width: 200px;
        }

        input[type="submit"], input[type="reset"] {
            width: 120px;
            margin: 10px;
            padding: 8px;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            background-color: #3498db;
            color: #fff;
        }

        input[type="reset"] {
            background-color: #e74c3c;
        }

        input[type="submit"]:hover {
            background-color: #2980b9;
        }

        input[type="reset"]:hover {
            background-color: #c0392b;
        }
    </style>
</head>
<body>

    <h2>فرم ثبت اطلاعات کاربر</h2>

    <form id="userForm">
        <div>
            <label for="nametext">نام:</label>
            <input id="nametext" type="text" name="name" required placeholder="مثلاً علی">
        </div>
        <div>
            <label for="familytext">نام خانوادگی:</label>
            <input id="familytext" type="text" name="family" required placeholder="مثلاً کرمی">
        </div>
        <div>
            <label>نوع اشتراک:</label>
            <select name="category">
                <option value="1">اشتراک یک‌ماهه</option>
                <option value="6">اشتراک شش‌ماهه</option>
                <option value="12">اشتراک یک‌ساله</option>
            </select>
        </div>
        <div>
            <label>تاریخ تولد:</label>
            <input type="date" name="bdate">
        </div>
        <div>
            <label>جنسیت:</label>
            <label>
                <input type="radio" name="gender" value="مذکر"> مذکر
            </label>
            <label>
                <input type="radio" name="gender" value="مونث"> مونث
            </label>
        </div>
        <div>
            <label>
                <input type="checkbox" name="check" required> موافقت با توافق‌نامه
            </label>
        </div>

        <br>
        <input type="reset" value="پاک کردن فرم">
        <input type="submit" value="ارسال">
    </form>

</body>
</html>
