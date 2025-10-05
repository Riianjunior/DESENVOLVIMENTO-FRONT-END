# DESENVOLVIMENTO-FRONT-END
<canvas id="graficoRecursos" width="400" height="400"></canvas>
<script>
  const ctx = document.getElementById('graficoRecursos');
  new Chart(ctx, {
    type: 'pie',
    data: {
      labels: ['Educação', 'Saúde', 'Meio Ambiente', 'Cultura'],
      datasets: [{
        data: [40, 25, 20, 15],
        backgroundColor: ['#4CAF50', '#2196F3', '#FFC107', '#E91E63']
      }]
    },
    options: {
      responsive: true,
      plugins: {
        legend: { position: 'bottom' },
        title: { display: true, text: 'Distribuição de Recursos por Projeto' }
      }
    }
  });
</script>

