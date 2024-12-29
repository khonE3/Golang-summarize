# Golang-Summarize (Not complete yet)


// Still learning for a long time //

Run file --> homeGo.go

# All commands basic Golang for amatures 


---

## 1. การประกาศตัวแปร

### ตัวอย่างโค้ด
```go
var folks string = "Folks"
var Npercent float32 = 95.2
const Persent = "%"

// การกำหนดค่าประเภทอัตโนมัติ
guys := "guys"

// การประกาศตัวแปรหลายตัวพร้อมกัน
var a, b, c int = 3, 8, 5
d, e, f := 1, 76.6, "Multiple influence Var"

// ค่าเริ่มต้นของตัวเลข
var F float32
```

### คำอธิบาย
- `var` ใช้สำหรับการประกาศตัวแปรที่มีการระบุชนิดข้อมูลอย่างชัดเจน
- `:=` ใช้สำหรับกำหนดค่าประเภทอัตโนมัติ
- ค่าคงที่ (`const`) ไม่สามารถเปลี่ยนแปลงค่าได้

---

## 2. การพิมพ์ข้อมูล

### ตัวอย่างโค้ด
```go
fmt.Println("Hola", folks, Npercent, Persent)
fmt.Println("Como estas?", guys)
fmt.Println("Multiple Var", a, b, c)
fmt.Println(d, e, f)

fmt.Printf("\"ค่าDefaultตัวเลขคือ %v\" Typeคือ%T\n", F, F)
```

### คำอธิบาย
- `fmt.Println` ใช้สำหรับพิมพ์ข้อมูลพร้อมขึ้นบรรทัดใหม่
- `fmt.Printf` รองรับการจัดรูปแบบข้อความ
  - `%v`: แสดงค่าของตัวแปร
  - `%T`: แสดงชนิดข้อมูลของตัวแปร

---

## 3. อาร์เรย์

### ตัวอย่างโค้ด
```go
var section = [3]int{1, 2, 3}
unknowsection := [...]string{"one", "two", "three", "four"}

SizeOfAarrylen := len(unknowsection)

fmt.Println(section)
fmt.Println(unknowsection)
fmt.Println(unknowsection[2])
fmt.Println("จำนวนarrayมี", SizeOfAarrylen, "ตัว")
```

### คำอธิบาย
- อาร์เรย์ใน Go มีขนาดคงที่และเก็บข้อมูลเป็นกลุ่มของสมาชิก
- `len()` ใช้สำหรับตรวจสอบขนาดของอาร์เรย์
- สัญลักษณ์ `...` ให้ Go กำหนดขนาดอาร์เรย์จากจำนวนสมาชิก

---

## 4. การรับข้อมูลจากผู้ใช้

### ตัวอย่างโค้ด
```go
var Scan_f string = "Scanf"
fmt.Print("ป้อนข้อความเพื่อแสดงผล = ")
fmt.Scanf("%s\n", &Scan_f)
fmt.Println("ข้อความของคุณ =", Scan_f)
```

### คำอธิบาย
- `fmt.Scanf` ใช้สำหรับอ่านข้อมูลจากผู้ใช้
  - `%s`: อ่านค่าเป็นข้อความ (string)
  - `&`: ส่งต่อที่อยู่หน่วยความจำของตัวแปรเพื่อเก็บค่า
- ใช้ `\n` ในรูปแบบเพื่ออ่านค่าทีละบรรทัด

---

## 5. โครงสร้างควบคุม

### ตัวอย่างโค้ด
```go
var banks int
fmt.Print("เลือก 1 หรือ 2 เพื่อทำรายการ ")
fmt.Scanf("%d", &banks)
if banks == 1 {
    fmt.Println("1.ฝากเงิน")
} else if banks == 2 {
    fmt.Println("2.ถอนเงิน")
} else {
    fmt.Println("อย่ากรอกมั่ว")
}
```

### คำอธิบาย
- `if-else` ใช้สำหรับการตรวจสอบเงื่อนไข
- เงื่อนไขจะประเมินเป็น `true` หรือ `false`

---


