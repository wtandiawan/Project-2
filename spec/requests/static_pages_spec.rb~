require 'spec_helper'

describe "Static pages" do

  subject { page }

  describe "Home page" do
    before { visit root_path }

    it { should have_content('Universe') }
    it { should have_title(full_title('')) }
    it { should_not have_title('| Home') }
  end

  describe "Faq page" do
    before { visit faq_path }

    it { should have_content('FAQ') }
    it { should have_title(full_title('Frequently Asked Questions')) }
  end

  describe "About page" do
    before { visit about_path }

    it { should have_content('About') }
    it { should have_title(full_title('About Me')) }
  end

  describe "Blog page" do
    before { visit blog_path }

    it { should have_content('BLOG') }
    it { should have_title(full_title('Blog')) }
  end
end
