// 1. feladat

const dobasok = [3, 1, 1, 2, 1, 5, 5, 4, 4, 4, 1, 2, 3, 6, 4, 6, 1, 4];


// 2. feladat

console.log("2. feladat");

let pozicio = 0;
let visszalepesek = 0;

for (let dobas of dobasok) {
    pozicio += dobas;

    // Létra mező
    if (pozicio % 10 === 0) {
        pozicio -= 3;
        visszalepesek++;
    }

    process.stdout.write(pozicio + " ");
}

console.log("\n");


// 3. feladat

console.log("3. feladat");
console.log(`A játék során ${visszalepesek} alkalommal lépett létrára.`);


// 4. feladat

console.log("4. feladat");

if (pozicio >= 45) {
    console.log("A játék befejezte.");
} else {
    console.log("A játékot abbahagyta.");
}
