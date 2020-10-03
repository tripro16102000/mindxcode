# mindxcode
//Ex1
let weight = Number(prompt(`Please enter your weight(kg)`));
console.log(weight);
let heightCm = Number(prompt(`Please enter your height(cm)`));
console.log(heightCm);
let heightM = heightCm / 100;
console.log(heightM);
let bmi = weight / (heightM * heightM);
if (bmi<16){
    console.log("Severely underweight");
}else if (16<= bmi && bmi<=18.5){
    console.log("Underweight");
}else if (18.5<bmi && bmi<=25){
    console.log("Normal");
}else if (25<bmi && bmi<=30){
    console.log("Overweight");
}else {
    console.log("Obese");
}
//Ex2
let userNumber = Number(prompt("Enter your number"));
if (userNumber<0){
    console.log("It does not exist");
}else if (userNumber === 0){
    console.log(`The factorial of ${userNumber} is 1`);
}else{
    let fact = 1
    for (i = 1; i <= userNumber; i++){
        fact *= i;
    }
    console.log(`The facorial of ${userNumber} is ${fact}`);
}
