<template>
    <div>
        <h1>Calculadora Aritmética</h1>
        <h3>- Para utilizar a calculadora, comece inserindo o primeiro valor numérico no campo indicado.</h3>
        <h3>- Em seguida, selecione a operação desejada – soma, subtração, multiplicação ou divisão – a partir do menu suspenso.</h3>
        <h3>- Após escolher a operação, digite o segundo número no próximo campo. Assim que ambos os números e a operação estiverem definidos, a calculadora processará automaticamente e exibirá o resultado da operação escolhida.</h3>

        <input type="number" v-model.number="numero1">
        <select v-model="operacao">
            <option value="adicao">+</option>
            <option value="subtracao">-</option>
            <option value="multiplicacao">*</option>
            <option value="divisao">/</option>
        </select>
        <input type="number" v-model.number="numero2">

        <p>Resultado: {{ resultado }}</p>
    </div>
</template>

<script>
export default {
    data() {
        return {
            numero1: 0,
            numero2: 0,
            operacao: 'adicao',
        };
    },
    computed: {
        resultado() {
            switch (this.operacao) {
                case 'adicao':
                    return this.numero1 + this.numero2;
                case 'subtracao':
                    return this.numero1 - this.numero2;
                case 'multiplicacao':
                    return this.numero1 * this.numero2;
                case 'divisao':
                    return this.numero2 !== 0 ? this.numero1 / this.numero2 : 'Divisão por zero!';
                default:
                    return 0;
            }
        },
    },
};
</script>
