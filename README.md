# Golang-Summarize (Not complete yet)


// Still learning for a long time //

Run file --> homeGo.go

# All commands basic Golang for amatures 

 
  
	var folks string = "Folks"
	var Npercent float32 = 95.2
	const Persent = "%"

	//* Type influence Var
	guys := "guys"

	//* Multiple Var
	var a, b, c int = 3, 8, 5
	d, e, f := 1, 76.6, "Multiple influence Var"

	var F float32

	//* PrintLine
	fmt.Println("Hola", folks, Npercent, Persent)
	fmt.Println("Como estas?", guys)
	fmt.Println("Multiple Var", a, b, c)
	fmt.Println(d, e, f)

	//* PrintFunction
	fmt.Printf("\"ค่าDefaultตัวเลขคือ %v\" Typeคือ%T\n", F, F)
	//! %v คือ ตัวแปรvar  %T คือ ตัวType

	//* Array
	//TODO ปรับเปลี่ยนขนาดสมาชิกไม่ได้
	//! var array_name = [length]datatype{values}
	//! array_name := [...]datatype{values}
	var section = [3]int{1, 2, 3}
	unknowsection := [...]string{"one", "two", "three", "four"}
	//? len() จำนวนindexของarray
	SizeOfAarrylen := len(unknowsection)

	fmt.Println(section)
	fmt.Println(unknowsection)
	fmt.Println(unknowsection[2])
	fmt.Println("จำนวนarrayมี ", SizeOfAarrylen, " ตัว ")

	//* Scanf
	//! string_format = รูปแบบตัวแทนชนิดข้อมูล
	//! address_list (&)
	var Scan_f string = "Scanf"
	fmt.Print("ป้อนข้อความเพื่อแสดงผล = ")
	fmt.Scanf("%s\n", &Scan_f)
	//? ใช้ \n เพื่อรับค่าทีละตัว
	fmt.Println("่ข้อความของคุณ = ", Scan_f)

	//* If else
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
