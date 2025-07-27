body {
    font-family: 'Kanit', sans-serif; /* ใช้ฟอนต์ Kanit หรือฟอนต์ sans-serif อื่นๆ */
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
    color: #333;
    line-height: 1.6;
}

header {
    background-color: #333;
    color: #fff;
    padding: 1rem 0;
    text-align: center;
    box-shadow: 0 2px 5px rgba(0,0,0,0.2);
}

header h1 {
    margin: 0;
    font-size: 2.5em;
}

header p {
    font-size: 1.1em;
    opacity: 0.9;
}

nav {
    background-color: #555;
    padding: 0.8rem 0;
    text-align: center;
}

nav ul {
    list-style: none;
    padding: 0;
    margin: 0;
    display: flex;
    justify-content: center;
    flex-wrap: wrap; /* ให้เมนูขึ้นบรรทัดใหม่ได้เมื่อหน้าจอเล็ก */
}

nav ul li {
    margin: 0 15px;
}

nav ul li a {
    color: #fff;
    text-decoration: none;
    font-weight: bold;
    padding: 5px 10px;
    border-radius: 5px;
    transition: background-color 0.3s ease;
}

nav ul li a:hover {
    background-color: #777;
}

main {
    padding: 20px;
    max-width: 1200px;
    margin: 20px auto;
    background-color: #fff;
    border-radius: 8px;
    box-shadow: 0 0 10px rgba(0,0,0,0.1);
}

.sport-section {
    margin-bottom: 40px;
    padding-bottom: 20px;
    border-bottom: 1px solid #eee;
}

.sport-section:last-child {
    border-bottom: none;
}

.sport-section h2 {
    color: #007bff;
    text-align: center;
    margin-bottom: 25px;
    font-size: 2em;
    position: relative;
    padding-bottom: 10px;
}

.sport-section h2::after {
    content: '';
    position: absolute;
    left: 50%;
    bottom: 0;
    transform: translateX(-50%);
    width: 60px;
    height: 3px;
    background-color: #007bff;
    border-radius: 2px;
}

.sport-content {
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    gap: 20px;
}

.sport-content img {
    width: 100%;
    max-width: 400px; /* กำหนดขนาดสูงสุดของรูปภาพ */
    height: auto;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0,0,0,0.1);
    object-fit: cover; /* ทำให้รูปภาพพอดีกับขนาดที่กำหนดโดยไม่บิดเบี้ยว */
    flex-shrink: 0; /* ป้องกันไม่ให้รูปภาพหดตัว */
}

.sport-content p {
    flex: 1; /* ทำให้ p ขยายเต็มพื้นที่ที่เหลือ */
    min-width: 300px; /* กำหนดขนาดขั้นต่ำของข้อความเมื่อหน้าจอเล็ก */
}

footer {
    background-color: #333;
    color: #fff;
    text-align: center;
    padding: 1rem 0;
    margin-top: 30px;
    box-shadow: 0 -2px 5px rgba(0,0,0,0.2);
}

/* Responsive adjustments */
@media (max-width: 768px) {
    nav ul {
        flex-direction: column;
        align-items: center;
    }

    nav ul li {
        margin: 5px 0;
    }

    .sport-content {
        flex-direction: column;
        text-align: center;
    }

    .sport-content img {
        max-width: 100%;
    }
}

@media (max-width: 480px) {
    header h1 {
        font-size: 2em;
    }

    header p {
        font-size: 1em;
    }

    .sport-section h2 {
        font-size: 1.8em;
    }
}
