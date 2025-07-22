<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Indicadores de Desempenho 2021-2025 | Departamento de Controle de Incentivos</title>
    
    <script src="https://cdn.jsdelivr.net/npm/apexcharts"></script>
    
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700&display=swap" rel="stylesheet">

    <style>
        /* --- Estilos Gerais e Reset --- */
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f4f7fa;
            color: #333;
            margin: 0;
            padding: 20px;
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        /* --- Cabeçalho da Página --- */
        header {
            text-align: center;
            margin-bottom: 40px;
            width: 100%;
            max-width: 1200px;
        }

        header h1 {
            color: #1a253c;
            font-size: 2.5rem;
            margin: 0;
        }

        header p {
            color: #5a6a85;
            font-size: 1.1rem;
            margin-top: 8px;
        }

        /* --- Contentor Principal e Grelha de Gráficos --- */
        main {
            width: 100%;
            max-width: 1200px;
            display: grid;
            grid-template-columns: repeat(2, 1fr); /* Grelha 2x2 para desktops */
            gap: 25px;
        }

        /* --- Estilo dos Cartões (Cards) que contêm os gráficos e a tabela --- */
       .card {
            background-color: #ffffff;
            border-radius: 8px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.05);
            padding: 20px;
            transition: transform 0.2s ease-in-out, box-shadow 0.2s ease-in-out;
        }

       .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.08);
        }
        
        /* Ocupa a largura total da grelha */
       .full-width {
            grid-column: 1 / -1;
        }

        /* --- Tabela de Dados --- */
       .data-table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 10px;
        }

       .data-table caption {
            font-size: 0.9em;
            color: #777;
            padding-bottom: 10px;
            caption-side: bottom;
            text-align: center;
        }

       .data-table th,.data-table td {
            padding: 12px 15px;
            text-align: left;
            border-bottom: 1px solid #e0e0e0;
        }

       .data-table thead th {
            background-color: #f8f9fa;
            font-weight: 500;
            color: #1a253c;
        }
        
       .data-table tbody tr:hover {
            background-color: #f1f1f1;
        }
        
       .data-table tfoot td {
            font-style: italic;
            color: #777;
            font-size: 0.9em;
            text-align: center;
            padding-top: 15px;
            border-bottom: none;
        }


        /* --- Rodapé da Página --- */
        footer {
            margin-top: 40px;
            padding-top: 20px;
            border-top: 1px solid #e0e0e0;
            width: 100%;
            max-width: 1200px;
            text-align: center;
            color: #777;
        }
        
        footer .disclaimer {
            font-weight: 500;
            color: #d9534f; /* Tom de vermelho para destaque */
        }

        /* --- Media Queries para Responsividade --- */
        @media (max-width: 992px) {
            main {
                grid-template-columns: 1fr; /* Grelha de 1 coluna para tablets e telemóveis */
            }
            header h1 {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>

    <header>
        <h1>Indicadores de Desempenho 2021-2025</h1>
        <p>Departamento de Controle de Incentivos | Secretaria Executiva de Desenvolvimento Econômico</p>
    </header>

    <main>
        <div class="card full-width" id="chart-empresas-mao-de-obra"></div>

        <div class="card" id="chart-projetos-aprovados"></div>

        <div class="card" id="chart-investimento"></div>
        
        <div class="card full-width">
            <h2>Dados Consolidados</h2>
            <table class="data-table">
                <caption>Tabela de dados consolidados dos indicadores de desempenho de 2021 a 2025.</caption>
                <thead>
                    <tr>
                        <th>Indicador</th>
                        <th>2021</th>
                        <th>2022</th>
                        <th>2023</th>
                        <th>2024</th>
                        <th>2025*</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>Empresas Incentivadas</td>
                        <td>527</td>
                        <td>633</td>
                        <td>656</td>
                        <td>692</td>
                        <td>672</td>
                    </tr>
                    <tr>
                        <td>Mão de Obra</td>
                        <td>95.573</td>
                        <td>99.007</td>
                        <td>101.534</td>
                        <td>114.119</td>
                        <td>116.535</td>
                    </tr>
                    <tr>
                        <td>Projetos Aprovados</td>
                        <td>216</td>
                        <td>254</td>
                        <td>257</td>
                        <td>263</td>
                        <td>125</td>
                    </tr>
                    <tr>
                        <td>Investimento Projetado (R$ Bilhões)</td>
                        <td>19,9</td>
                        <td>8,3</td>
                        <td>5,1</td>
                        <td>6,9</td>
                        <td>4,3</td>
                    </tr>
                </tbody>
                <tfoot>
                    <tr>
                        <td colspan="6">*Valores de 2025 parciais, referentes ao período até Junho.</td>
                    </tr>
                </tfoot>
            </table>
        </div>
    </main>

    <footer>
        <p>Fonte: Departamento de Controle de Incentivos.</p>
        <p class="disclaimer">Nota Importante: Os dados referentes ao ano de 2025 são parciais e cobrem o período até 30 de Junho de 2025.</p>
    </footer>

    <script>
        // Espera o DOM ser totalmente carregado para executar os scripts dos gráficos
        document.addEventListener("DOMContentLoaded", function() {
            
            // --- DADOS GERAIS ---
            const anos = ['2021', '2022', '2023', '2024', '2025*'];
            const cores = {
                azul: '#008FFB',
                verde: '#00E396',
                amarelo: '#FEB019',
                vermelho: '#FF4560',
                cinzaParcial: '#A9A9A9'
            };

            // --- GRÁFICO 1: Empresas Incentivadas vs. Mão de Obra (Gráfico Misto) ---
            const optionsEmpresasMaoDeObra = {
                // Define as séries de dados. Cada objeto representa uma métrica.
                series: [{
                    name: 'Empresas Incentivadas',
                    type: 'column', // Tipo de gráfico: coluna
                    data: [527, 633, 656, 692, 672] 
                }, {
                    name: 'Mão de Obra',
                    type: 'line', // Tipo de gráfico: linha
                    data: [95573, 99007, 101534, 114119, 116535]
                }],
                chart: {
                    height: 350,
                    type: 'line', // Tipo base do gráfico
                    toolbar: { show: true },
                    zoom: { enabled: false }
                },
                stroke: {
                    width: [0, 4], // Largura do traço: 0 para colunas, 4 para a linha
                    curve: 'smooth' // Curva da linha suave
                },
                title: {
                    text: 'Crescimento de Empresas Incentivadas e Mão de Obra',
                    align: 'left'
                },
                // Rótulos de dados desativados para um visual mais limpo, a informação está na tooltip
                dataLabels: {
                    enabled: false,
                },
                // Define os rótulos do eixo X (horizontal)
                xaxis: {
                    categories: anos
                },
                // Configuração dos dois eixos Y (vertical) para escalas diferentes
                yaxis: [{
                    title: {
                        text: 'Quantidade de Empresas',
                    },
                }, {
                    opposite: true, // Coloca este eixo do lado direito
                    title: {
                        text: 'Mão de Obra Total'
                    },
                     labels: {
                        formatter: (val) => { return val.toLocaleString('pt-BR'); }
                    }
                }],
                tooltip: {
                    shared: true, // Mostra os dados de ambas as séries ao passar o mouse
                    intersect: false,
                    y: {
                        formatter: function (y) {
                            if (typeof y !== "undefined") {
                                return y.toLocaleString('pt-BR') + " ";
                            }
                            return y;
                        }
                    }
                },
                legend: {
                    position: 'top',
                    horizontalAlign: 'right'
                },
                colors: [cores.azul, cores.verde]
            };

            const chartEmpresasMaoDeObra = new ApexCharts(document.querySelector("#chart-empresas-mao-de-obra"), optionsEmpresasMaoDeObra);
            chartEmpresasMaoDeObra.render();


            // --- GRÁFICO 2: Projetos Aprovados (Gráfico de Área com Anotação) ---
            const optionsProjetosAprovados = {
                series: [{
                    name: 'Projetos Aprovados',
                    data: [216, 254, 257, 263, 125]
                }],
                chart: {
                    height: 350,
                    type: 'area',
                    toolbar: { show: false }
                },
                // Anotação para destacar o dado parcial de 2025
                annotations: {
                    points: [{
                        x: '2025*', // O valor no eixo X para anotar
                        seriesIndex: 0,
                        label: {
                            borderColor: cores.amarelo,
                            offsetY: 0,
                            style: {
                                color: '#fff',
                                background: cores.amarelo,
                            },
                            text: 'Parcial',
                        }
                    }]
                },
                dataLabels: {
                    enabled: true // Mostra os valores em cada ponto
                },
                stroke: {
                    curve: 'smooth'
                },
                xaxis: {
                    categories: anos
                },
                yaxis: {
                    title: {
                        text: 'Quantidade de Projetos'
                    }
                },
                title: {
                    text: 'Total de Projetos Aprovados por Ano',
                    align: 'left'
                },
                colors: [cores.amarelo]
            };

            const chartProjetosAprovados = new ApexCharts(document.querySelector("#chart-projetos-aprovados"), optionsProjetosAprovados);
            chartProjetosAprovados.render();


            // --- GRÁFICO 3: Investimento Projetado (Gráfico de Barras Horizontais) ---
            const optionsInvestimento = {
                series: [{
                    name: 'Investimento Projetado',
                    data: [19.9, 8.3, 5.1, 6.9, 4.3]
                }],
                chart: {
                    type: 'bar',
                    height: 350,
                    toolbar: { show: false }
                },
                plotOptions: {
                    bar: {
                        horizontal: true, // Define o gráfico como horizontal
                        dataLabels: {
                            position: 'top', // Posição dos rótulos de dados
                        },
                    }
                },
                dataLabels: {
                    enabled: true,
                    offsetX: -6,
                    style: {
                        fontSize: '12px',
                        colors: ['#fff']
                    },
                    formatter: (val) => { return val.toFixed(1).replace('.', ',') + " B"; } // Formata o valor
                },
                stroke: {
                    show: true,
                    width: 1,
                    colors: ['#fff']
                },
                xaxis: {
                    categories: anos,
                    title: {
                        text: 'R$ (em Bilhões)'
                    }
                },
                yaxis: {
                    labels: {
                        show: true
                    }
                },
                title: {
                    text: 'Investimento Projetado Anual',
                    align: 'left'
                },
                // Coloração condicional: a barra de 2025 terá uma cor diferente
                colors: [function({ value, seriesIndex, dataPointIndex, w }) {
                    if (dataPointIndex === 4) { // Índice 4 corresponde a 2025
                        return cores.cinzaParcial;
                    } else {
                        return cores.vermelho;
                    }
                }],
                tooltip: {
                    y: {
                        formatter: function (val) {
                            return "R$ " + val.toFixed(1).replace('.', ',') + " Bilhões";
                        }
                    }
                }
            };
            
            const chartInvestimento = new ApexCharts(document.querySelector("#chart-investimento"), optionsInvestimento);
            chartInvestimento.render();

        });
    </script>
</body>
</html>
