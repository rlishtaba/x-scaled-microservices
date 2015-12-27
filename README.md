# X-axis scaling as a typical horizontal scaling pattern in microservices architecture

Practical example of microservices architecture using Docker infrastructure. 

## Bootstrap

Replace an IP addresses in the root "docker-compose.yml" with appropriate ones according to your infrastructure. Make sure "consul" UDP port should be bound to docker's `docker0` network interface (run `docker-machine ssh {environment}` and then inspect interface details with `ifconfig docker0` command).

	docker-compose up -d

## Scale

	docker-compose scale web=3

## UI 

Consul UI: http://{dockerhost}:8500

Load Balancer: http://{dockerhost}:8080	

##Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/rlishtaba/x-scaled-microservices. This project is intended to be a safe, welcoming space for collaboration, and contributors are expected to adhere to the Contributor Covenant code of conduct.

##License

The library is available as open source under the terms of the MIT License.