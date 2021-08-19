---
layout: page
title: Request Free License
permalink: /free/
---

The free license is only usable in a personal and non-commercial context. Commercial use of Bug Shooting requires the purchasing of a [commercial license]({{ site.baseurl }}/buy).

<div class="container">
  
      <div class="row">
      <div class="form-group">
        <label for="txtFirstName" class="col-sm-3 control-label"><%=Resources.Language.Purchase_FirstName %></label>
        <div class="col-sm-9">
          <asp:TextBox ID="txtFirstName" CssClass="form-control" runat="server" />
          <div class="help-block with-errors pull-right"></div>
          <span class="form-control-feedback" aria-hidden="true"></span>
        </div>
      </div>
      <div class="form-group">
        <label for="txtLastName" class="col-sm-3 control-label"><%=Resources.Language.Purchase_LastName %></label>
        <div class="col-sm-9">
          <asp:TextBox ID="txtLastName" CssClass="form-control" runat="server" />
          <div class="help-block with-errors pull-right"></div>
          <span class="form-control-feedback" aria-hidden="true"></span>
        </div>
      </div>
      <div class="form-group">
        <label for="txtEmail" class="col-sm-3 control-label"><%=Resources.Language.Email %></label>
        <div class="col-sm-9">
          <asp:TextBox ID="txtEmail" CssClass="form-control" runat="server" AutoCompleteType="Email" />
          <div class="help-block with-errors pull-right"></div>
          <span class="form-control-feedback" aria-hidden="true"></span>
        </div>
      </div>
      <div class="form-group">
        <label for="txtEmailRepeat" class="col-sm-3 control-label"><%=Resources.Language.Email_Repeat %></label>
        <div class="col-sm-9">
          <asp:TextBox ID="txtEmailRepeat" CssClass="form-control" runat="server" AutoCompleteType="Email" />
          <div class="help-block with-errors pull-right"></div>
          <span class="form-control-feedback" aria-hidden="true"></span>
        </div>
      </div>
      <div class="form-group">
        <label for="txtCountry" class="col-sm-3 control-label"><%=Resources.Language.Purchase_Country %></label>
        <div class="col-sm-9">
          <asp:TextBox ID="txtCountry" CssClass="form-control" runat="server" />
          <div class="help-block with-errors pull-right"></div>
          <span class="form-control-feedback" aria-hidden="true"></span>
        </div>
      </div>
      <div class="form-group">
        <label for="txtCity" class="col-sm-3 control-label"><%=Resources.Language.Purchase_City %></label>
        <div class="col-sm-9">
          <asp:TextBox ID="txtCity" CssClass="form-control" runat="server" />
          <div class="help-block with-errors pull-right"></div>
          <span class="form-control-feedback" aria-hidden="true"></span>
        </div>
      </div>
      <div class="form-group">
        <label for="txtZip" class="col-sm-3 control-label"><%=Resources.Language.Purchase_Zip %></label>
        <div class="col-sm-9">
          <asp:TextBox ID="txtZip" CssClass="form-control" runat="server" />
          <div class="help-block with-errors pull-right"></div>
          <span class="form-control-feedback" aria-hidden="true"></span>
        </div>
      </div>
      <div class="form-group">
        <label for="txtStreet" class="col-sm-3 control-label"><%=Resources.Language.Purchase_Street %></label>
        <div class="col-sm-9">
          <asp:TextBox ID="txtStreet" CssClass="form-control" runat="server" />
          <div class="help-block with-errors pull-right"></div>
          <span class="form-control-feedback" aria-hidden="true"></span>
        </div>
      </div>
      <div class="form-group">
        <label for="txtCaptchaImageCode" class="col-sm-3 control-label"><%=Resources.Language.Captcha %></label>
        <div class="col-sm-9">
          <asp:TextBox ID="txtCaptchaImageCode" CssClass="form-control" runat="server" />
          <div class="help-block with-errors pull-right"></div>
          <span class="form-control-feedback" aria-hidden="true"></span>
        </div>
      </div>
      <div class="form-group">
        <div class="col-sm-offset-3 col-sm-9">
          <asp:CheckBox ID="chkAcceptLicense" runat="server" />
          <div class="help-block with-errors pull-right"></div>
          <span class="form-control-feedback" aria-hidden="true"></span>
        </div>
      </div>
      <div class="form-group">
        <div class="col-sm-offset-3 col-sm-9">
          <asp:LinkButton ID="cmdRequest" CssClass="btn btn-yellow pull-right" runat="server" ><%=Resources.Language.Request_Free_License%></asp:LinkButton>
        </div>
      </div>

    </div>

  </div>
