# No terminal:
git clone https://github.com/helvsroots/quantum-trading
cd quantum-trading
npm install
git add .
git commit -m "Initial commit"
// src/components/SentimentoHoje.js
import React from 'react';
export default function SentimentoHoje() {
  return (
    <div className="min-h-screen bg-gradient-to-br from-gray-900 to-gray-800 flex items-center justify-center p-4">
      <div className="max-w-2xl w-full bg-gray-900/80 backdrop-blur-lg rounded-2xl p-8 border border-gray-700 shadow-2xl">
        {/* Cabeçalho */}
        <div className="text-center mb-8">
          <h1 className="text-4xl font-bold bg-gradient-to-r from-red-500 to-orange-500 bg-clip-text text-transparent">
            QUANTUM TRADING
          </h1>
          <p className="mt-2 text-gray-400">Análise Quântica do Mercado em Tempo Real</p>
        </div>

        {/* Card de Sentimento */}
        <div className="bg-gray-800 rounded-xl p-6 mb-6 animate-pulse">
          <div className="flex items-center justify-between">
            <span className="text-sm text-gray-400">Atualizado em 12/03/2025 09:00</span>
            <span className="px-4 py-1 bg-red-500/20 text-red-500 rounded-full text-sm">
              AO VIVO
            </span>
          </div>
          
          <div className="mt-4">
            <h2 className="text-2xl font-bold text-red-500 flex items-center gap-2">
              🔥 BEARISH 
              <span className="text-lg text-gray-400">(65% probabilidade)</span>
            </h2>
          </div>
        </div>

        {/* Grid de Ativos */}
        <div className="grid grid-cols-1 md:grid-cols-2 gap-4">
          {/* IBOVESPA */}
          <div className="bg-gray-800 p-6 rounded-xl">
            <h3 className="text-lg font-bold flex items-center gap-2">
              <span className="text-blue-400">📉</span>
              IBOVESPA
            </h3>
            <div className="mt-4 space-y-2">
              <p className="text-2xl font-bold">148.500 <span className="text-red-500 text-lg">(-2.1%)</span></p>
              <div className="flex justify-between text-sm text-gray-400">
                <span>Suporte: 145.000</span>
                <span>Resistência: 152.000</span>
              </div>
            </div>
          </div>

          {/* DÓLAR */}
          <div className="bg-gray-800 p-6 rounded-xl">
            <h3 className="text-lg font-bold flex items-center gap-2">
              <span className="text-green-400">💸</span>
              DÓLAR (WDO)
            </h3>
            <div className="mt-4 space-y-2">
              <p className="text-2xl font-bold">R$ 6,02 <span className="text-green-500 text-lg">(+2.3%)</span></p>
              <div className="flex justify-between text-sm text-gray-400">
                <span>PTAX: 5,95</span>
                <span>Ajuste: +0,12</span>
              </div>
            </div>
          </div>
        </div>

        {/* CTAs */}
        <div className="mt-8 flex flex-col gap-4">
          <a href="https://t.me/quantumtradingbot" 
             className="bg-blue-600 hover:bg-blue-700 text-center py-4 rounded-xl font-bold transition-all">
            📲 Receber Alertas no Telegram
          </a>
          
          <button className="bg-gray-700 hover:bg-gray-600 py-4 rounded-xl font-bold transition-all">
            📘 Guia Completo (PDF Premium)
          </button>
        </div>
      </div>
    </div>
  );
}

git push origin main
git clone https://github.com/helvsroots/quantum-trading
cd quantum-trading
git add .
git commit -m "Primeira versão do Quantum Trading"
git push origin main
