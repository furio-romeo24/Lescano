int columnas = 10;
int filas = 10;

int tam = 50;

boolean[][][] celdas;

void setup() {
  size(500, 500);

  celdas = new boolean[columnas][filas][6];

  generarLaberinto();
}

void draw() {
  background(255);

  dibujarLaberinto();
}

void generarLaberinto() {

  for (int x = 0; x < columnas; x++) {
    for (int y = 0; y < filas; y++) {

      for (int i = 0; i < 6; i++) {

        celdas[x][y][i] = random(1) > 0.5;
      }
    }
  }
}

void dibujarLaberinto() {

  stroke(0);

  for (int x = 0; x < columnas; x++) {
    for (int y = 0; y < filas; y++) {

      int px = x * tam;
      int py = y * tam;

      if (celdas[x][y][0]) {
        line(px, py, px + tam, py);
      }

      if (celdas[x][y][1]) {
        line(px + tam, py, px + tam, py + tam);
      }

      if (celdas[x][y][2]) {
        line(px + tam, py + tam, px, py + tam);
      }

      if (celdas[x][y][3]) {
        line(px, py + tam, px, py);
      }

      if (celdas[x][y][4]) {
        line(px, py, px + tam, py + tam);
      }

      if (celdas[x][y][5]) {
        line(px + tam, py, px, py + tam);
      }
    }
  }
}
