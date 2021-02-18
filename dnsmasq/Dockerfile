FROM alpine:3.13
RUN apk --no-cache add dnsmasq-dnssec
COPY ./trust-anchors.conf /etc/trust-anchors.conf
EXPOSE 53 53/udp
EXPOSE 57 57/udp
EXPOSE 69 69/udp
ENTRYPOINT ["dnsmasq", "-k"]
