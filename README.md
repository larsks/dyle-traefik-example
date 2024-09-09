Start traefik:

    (cd traefik && docker compose up -d)

Start fake mailpit container:

    (cd mailpit && docker compose build && docker compose up -d)

Access the `whoami` service:

    curl -k https://localhost:8443/whoami

Access the `mailpit` service:

    curl -k https://localhost:8443/mailpit
