FROM prom/prometheus:latest

# Copy konfigurasi prometheus
COPY prometheus.yml /etc/prometheus/prometheus.yml

# Expose port 9090
EXPOSE 9090

# Set user prometheus
USER prometheus

# Command untuk menjalankan prometheus
CMD ["--config.file=/etc/prometheus/prometheus.yml", \
     "--storage.tsdb.path=/prometheus", \
     "--web.console.libraries=/usr/share/prometheus/console_libraries", \
     "--web.console.templates=/usr/share/prometheus/consoles"]
