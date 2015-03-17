A project that integrates [Phoenix](http://github.com/phoenixframework/phoenix) with [Ecto](http://github.com/elixir-lang/ecto), implementing all relevant protocols.

## Usage

You can use `phoenix_ecto` in your projects in two steps:

1. Add it to your `mix.exs` dependencies:

    ```elixir
    def deps do
      [{:phoenix_ecto, "~> 0.1.0"}]
    end
    ```

2. List it as your application dependency:

    ```elixir
    def application do
      [applications: [:logger, :phoenix_ecto]]
    end
    ```

## Details

This project:

  * Implements the `Phoenix.HTML.FormData` protocol for `Ecto.Changeset`
  * Implements the `Phoenix.HTML.Safe` protocol for `Decimal`
  * Implements the `Poison.Encoder` protocol for `Ecto.Date`, `Time` and
    `DateTime`

## License

Same license as Phoenix.
