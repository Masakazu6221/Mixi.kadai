# Mixi.kadai
class UsersController < ActionController
  def show
    user = User.find(params[:id].to_i)
    render json: user except[`cypted_password`]
  end
end
