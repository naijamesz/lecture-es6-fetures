## คุณสมบัติของ ES6

<a href="https://github.com/naijamesz/lecture-es6-fetures-EN-TH/blob/main/README-EN.md">English</a>

ES6 หรือ ECMAScript 2015 เป็นการอัปเดตที่สำคัญสำหรับภาษา JavaScript ที่นำเสนอคุณสมบัติใหม่มากมายเพื่อทำให้การเขียนโค้ดง่ายและมีประสิทธิภาพมากขึ้น นี่คือสรุปของคุณสมบัติหลักใน ES6 พร้อมตัวอย่างการใช้งาน:

1. **Let และ Const**

   - `let` ใช้ในการประกาศตัวแปรที่สามารถเปลี่ยนค่าได้
   - `const` ใช้ในการประกาศตัวแปรที่มีค่าคงที่
   - ตัวอย่าง:
     ```javascript
     let name = 'Alice';
     const PI = 3.14;
     ```

2. **Arrow Functions**

   - Arrow functions ให้สัญลักษณ์ที่สรุปสั้นกว่าในการกำหนดฟังก์ชัน
   - ตัวอย่าง:
     ```javascript
     const add = (a, b) => a + b;
     ```

3. **Template Literals**

   - Template literals ใช้เครื่องหมาย backticks (`` ` ``) เพื่อสร้างสตริงที่สามารถรวมตัวแปรและส่วนสูงสุดได้
   - ตัวอย่าง:
     ```javascript
     let name = 'Bob';
     console.log(`สวัสดี, ${name}!`);
     ```

4. **Destructuring Assignment**

   - Destructuring assignment ให้วิธีง่ายในการแยกค่าจากอาร์เรย์หรือคุณสมบัติจากออบเจกต์
   - ตัวอย่าง:
     ```javascript
     const [a, b] = [1, 2];
     const { x, y } = { x: 10, y: 20 };
     ```

5. **Default Parameters**

   - Default parameters ช่วยให้คุณกำหนดค่าเริ่มต้นสำหรับพารามิเตอร์ของฟังก์ชัน
   - ตัวอย่าง:
     ```javascript
     function greet(name = 'Guest') {
       console.log(`สวัสดี, ${name}!`);
     }
     ```

6. **Import/Export Modules**

   - Modules ช่วยให้คุณแบ่งโค้ดของคุณเป็นไฟล์ย่อยและนำเข้าหรือส่งออกฟังก์ชัน คลาส หรือตัวแปร
   - ตัวอย่าง:

     ```javascript
     // ไฟล์ math.js
     export const add = (a, b) => a + b;

     // ไฟล์ main.js
     import { add } from './math.js';
     console.log(add(2, 3));
     ```

7. **Promises และ Async/Await**

   - Promises และ async/await ให้วิธีในการจัดการกับการดำเนินการแบบไม่เชื่อมต่อ
   - ตัวอย่าง:
     ```javascript
     const fetchData = async () => {
       try {
         let response = await fetch('https://api.example.com/data');
         let data = await response.json();
         console.log(data);
       } catch (error) {
         console.error('ข้อผิดพลาด:', error);
       }
     };
     ```

8. **คลาส**

   - คลาสให้ไวยากรณ์ใหม่ในการสร้างออบเจกต์และการจัดการการสืบทอด
   - ตัวอย่าง:
     ```javascript
     class Person {
       constructor(name) {
         this.name = name;
       }
       greet() {
         console.log(`สวัสดี, ชื่อของฉันคือ ${this.name}`);
       }
     }
     ```

9. **เมธอดใหม่สำหรับวัตถุตระกูล**

   - เมธอดใหม่สำหรับวัตถุ อาร์เรย์ เป็นต้น
   - ตัวอย่าง:
     ```javascript
     Object.assign({}, { x: 1, y: 2 }); // {x: 1, y: 2}
     Array.from('foo'); // ['f', 'o', 'o']
     ```

10. **Spread/Rest Operator**

    - ตัวดำเนินการ `...` ใช้ในการกระจายองค์ประกอบของอาร์เรย์หรือออบเจกต์หรือรวบรวมพารามิเตอร์ในฟังก์ชัน
    - ตัวอย่าง:

      ```javascript
      const numbers = [1, 2, 3];
      const moreNumbers = [...numbers, 4, 5]; // [1, 2, 3, 4, 5]

      function sum(...args) {
        return args.reduce((acc, current) => acc + current, 0);
      }
      ```

ES6 นำเสนอคุณสมบัติที่ทำให้ JavaScript มีความสามารถและความยืดหยุ่นมากขึ้น เป็นการเปิดทางสำหรับการพัฒนา JavaScript ในอนาคต
