<script setup>
import { ref } from 'vue';
import '../src/css/carteira.css';
</script>

<template>
  <section id="main">
    <div class="container">
      <div class="painel-top">
        <div>
          <span>Carteira Financeira</span>
          <div class="box-saldo">R$ 1000,00</div>
          <span>Saldo</span>
        </div>

        <button>+ Adicionar</button>
      </div>

      <form class="box">
        <input type="number" placeholder="R$ 1.000,00" />
        <input type="text" placeholder="Descrição" />
        <select>
          <option value="">Selecione o tipo</option>
          <option value="Receita">Receita</option>
          <option value="Despesa">Despesa</option>
        </select>

        <button>Adicionar</button>
      </form>

      <div class="bar-search box">
        <h4>Movimentações</h4>
        <select class="select-filter">
          <option value="">Filtrar...</option>
          <option value="Receitas">Receitas</option>
          <option value="Despesas">Despesas</option>
        </select>
      </div>

      <ul class="list-transations box">
        <li>
          <p>Descrição</p>
          <span>Receita</span>
          <p>R$ 1000,00</p>
          <div class="actions">
            <button class="btn-remover">X</button>
            <button class="btn-editar">Editar</button>
          </div>
        </li>

        <li>
          <p>Descrição</p>
          <span>Receita</span>
          <p>R$ 1000,00</p>
          <div class="actions">
            <button class="btn-remover">X</button>
            <button class="btn-editar">Editar</button>
          </div>
        </li>
      </ul>

      <div class="box-pagination">
        <button><<</button>
        <span>1</span>
        <span class="separator">/</span>
        <span>5</span>
        <button>>></button>
      </div>
    </div>
  </section>
</template>
