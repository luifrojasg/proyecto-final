# Pokedex Lite

App móvil hecha con **React Native + TypeScript + Expo Router** que consume la [PokeAPI](https://pokeapi.co/).

## Pantallas (rutas)

| Ruta | Pantalla | Qué hace |
|------|----------|----------|
| `/` | Lista | Muestra los primeros 20 Pokémon |
| `/pokemon/[name]` | Detalle | Muestra imagen, tipos, altura, peso y estadísticas |

## Estructura

```
app/
├── _layout.tsx        ← navegación (Stack)
├── index.tsx          ← lista de Pokémon
└── pokemon/
    └── [name].tsx     ← detalle de un Pokémon
hooks/
├── usePokemonList.ts
└── usePokemonDetail.ts
types/
└── pokemon.ts         ← interfaces de TypeScript
```

## Cómo ejecutarlo

```bash
npm install
npx expo start
```

- Presiona `a` para abrir en el emulador Android (Plan A).
- Presiona `w` para abrir en el navegador (Plan B).

Si aparece un aviso de versiones de paquetes, corre `npx expo install --fix`.
