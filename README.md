# Kalman Folder Function Structure
This README provides the structure of the contents of this folder and a brief description of its usage.

    Kalman
    ├── _mou_car.py
    |   └── _mou_car                # Calculates parameters: Sigma_tilde, Q for the mOU CAR(p) process.
    ├── cov_car.py
    |   └── cov_car                 # Computes the covariance function for the CAR(p) process.
    ├── higher_mvncond.py
    |   └── higher_mvncond          # Computes the transition matrix and the variance matrix 
    |                                 in Y_{n+1} ~ p(Y_{n+1} | Y_n).
    ├── kalman_initial_draw.py
    |   └── kalman_initial_draw     # Computes the initial draw X_0 for the kalman process 
    |                                 given the initial value x_0.
    ├── kalman_ode_higher.py
    |   └── kalman_ode_higher       # Probabilistic ODE solver based on the Kalman filter and smoother. 
    |                                 Returns an approximate solution to the higher order ODE W*x_t = F(x_t, t).
    └── kalman_ode_higher.py
        ├── cov_vv_se           # Computes the covariance function for the derivative v_t 
        |                           using square exponential kernel. 
        ├── cov_xv_se           # Computes the cross-covariance function for the solution 
        |                         process x_t and its derivative v_t using square exponential kernel. 
        └── cov_xx_se           # Computes the covariance function for the solution process 
                                  x_t using square exponential kernel. 
                                  
