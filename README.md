# UF Token (ERC-20)

Este repositorio contiene el contrato inteligente del token UF, un token estándar ERC-20 en Ethereum, con una función especial de "mint" que solo puede ser utilizada por el dueño del contrato.

## Características

- Cumple con el estándar ERC-20.
- Nombre del token: UF
- Símbolo: UF
- Decimales: 18
- Función de "mint" (emisión de nuevos tokens) restringida únicamente al propietario del contrato.

## Funcionalidades principales

- Transferencia de tokens entre cuentas.
- Consulta de balances y suministro total.
- Aprobación y transferencia delegada.
- Emisión de nuevos tokens (mint) solo por el dueño.

## Ejemplo de función mint

```solidity
function mint(address to, uint256 amount) public onlyOwner {
    _mint(to, amount);
}
```

## Instalación

1. Clona este repositorio:
   ```bash
   git clone https://github.com/tuusuario/uf-token.git
   ```
2. Instala las dependencias necesarias (por ejemplo, usando Hardhat o Truffle).

## Despliegue

1. Configura tu archivo `.env` con las claves necesarias.
2. Ejecuta el script de despliegue con tu framework favorito.

## Licencia

Este proyecto está bajo la licencia MIT.
