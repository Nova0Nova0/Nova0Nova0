function convertir(cantidad, moneda) {
  // Definir los tipos de cambio
  let dolar = 10;
  let euro = 20;
  let bitcoin = 30;

  // Verificar la moneda y retornar la cantidad convertida
  if (moneda === 'dolar') {
    return cantidad * dolar;
  } else if (moneda === 'euro') {
    return cantidad * euro;
  } else if (moneda === 'bitcoin') {
    return cantidad * bitcoin;
  } else {
    return 'No existe tal moneda';
  }
}

// Ejemplos de uso
console.log(convertir(10, 'plata'));   // Salida: 'No existe tal moneda'
console.log(convertir(10, 'dolar'));   // Salida: 100
console.log(convertir(10, 'euro'));    // Salida: 200
console.log(convertir(10, 'bitcoin')); // Salida: 300
