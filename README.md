Foreman's export sets the `PORT` env incorrectly when both the PORT is present in .env and concurrency > 1 is used in the export command.

    foreman export -a bad_env -u me -e .env upstart . -c web=2
    foreman export -a good_env -u me -e .env upstart . -c web=2 -t templates
