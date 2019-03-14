---
layout: default
---
<div class="jumbotron-fluid">
  <div class="container">
    <div class="row">
      <div class="col-md"></div>
      <div class="col-md">
        <div class="h1 text-right text-primary">Host a hub</div>
      </div>
    </div>
    <div class="row">
      <div class="col-md"></div>
      <div class="col-md">
        <div class="h6 text-right">
          Become a member today and let the electric bike come to you. The more people sign up in your area, the faster we come!
        </div>
      </div>
    </div>
    <div class="row">
      <div class="col-md"></div>
      <div class="col-md">
        <form action="https://formspree.io/andersdalen@gmail.com" method="POST">
          <div class="form-row">
            <div class="col-lg-6">
            <div class="form-group">
              <!--label for="inputName">Name</label-->
              <input type="text" class="form-control" id="inputNumber" name="name" placeholder="Your name">
            </div>
            </div>
            <div class="col-lg-6">
            <div class="form-group">
              <!--label for="validationInputEmail">Email</label-->
              <input type="email" class="form-control is-invalid" id="validationInputEmail" name="_replyto" placeholder="Email (required)" required>
            </div>
            </div>
          </div>

          <div class="form-row">
            <div class="col-lg-4">
            <div class="form-group">
              <!--label for="inputStreet">Address</label-->
              <input type="text" class="form-control" id="inputStreet" placeholder="Address">
            </div>
            </div>
            <div class="col-lg-4">
            <div class="form-group">
              <!--label for="inputZip">Postal code</label-->
              <input type="number" class="form-control" id="inputZip" placeholder="Postal">
            </div>
            </div>
            <div class="col-lg-4">
            <div class="form-group">
              <!--label for="inputCity">City</label-->
              <input type="text" class="form-control" id="inputCity" placeholder="City">
            </div>
            </div>
          </div>
          <button type="submit" value="Send" class="btn btn-primary btn-block">Submit</button>
        </form>
        <p class="text-muted text-center">Powered by Formspree</p>
      </div>
    </div>
  </div>
</div>
